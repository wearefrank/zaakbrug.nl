<template>
    <div>
      <div :id="targetId"></div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HubspotForm',
    props: {
      portalId: {
        type: String,
        required: true
      },
      formId: {
        type: String,
        required: true
      },
      region: {
        type: String,
        default: 'na1'
      },
      targetId: {
        type: String,
        default: 'hubspot-form'
      }
    },
    mounted() {
      if (process.client) {
        if (!window.hbspt) {
          const script = document.createElement('script')
          script.src = '//js.hsforms.net/forms/embed/v2.js'
          script.charset = 'utf-8'
          script.async = true
          script.onload = this.createForm
          document.head.appendChild(script)
        } else {
          this.createForm()
        }
      }
    },
    methods: {
      createForm() {
        window.hbspt.forms.create({
          portalId: this.portalId,
          formId: this.formId,
          region: this.region,
          target: `#${this.targetId}`,
          onFormReady: (form) => {
            const input = form.querySelector('input[name="form_source_page"]')
            if (input) {
              input.value = "zaakbrug.nl" + window.location.pathname
            }
          }
        })
      }
    }
  }
  </script>
  