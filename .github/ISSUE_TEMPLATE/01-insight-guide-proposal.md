name: Insight Guide Proposal
about: Use this template to propose new CHAOSS Insight Guides
labels: ['insight guide', 'proposal']
assignees:
  - geekygirldawn

body:
  - type: markdown
    attributes:
      value: | 
        To avoid duplication and re-work, we ask you to use this template to propose new CHAOSS Insight Guides. While metrics models are designed with collections of metrics that can be implemented together, these Insight Guides are different from metrics models. Insight guides are designed to help us humans understand how to interpret metrics within a narrow topic and make improvements based on what is learned from that interpretation. Each Insight Guide should focus on 2-4 metrics, but can include a list of additional metrics in Step 3 - Gather Additional Data if needed.

  - type: markdown
    attributes:
      value: |
        ## Insight Guide Information

  - type: input
    attributes:
      label: Insight Guide Topic (1 - 3 words)
    validations:
      required: true

  - type: input
    attributes:
      label: Primary Metrics (2 - 4 metrics)
    validations:
      required: true

  - type: textarea
    attributes:
      label: Why is this topic important? How will this help people improve their open source project and / or community? Who will benefit from this guide?
    validations:
      required: true

  - type: dropdown
    attributes:
      label: How would you like to see this guide developed?
      options:
        - I have the experience and time available to write the first draft
        - I would like to help write the guide, but I need someone with more experience in the topic to help me
        - I am interested in using this guide, but I do not want to write it myself
        - Other (please specify in the “Additional Notes” at the end of this form)
    validations:
      required: true

  - type: textarea
    attributes:
      label: Additional Notes
    validations:
      required: true
