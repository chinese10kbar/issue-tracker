name: Bug Report
description: File a bug report
title: "[Bug]: "
labels: [bug, triage]
body:
  - type: markdown
    attributes:
      value: |
        Thank you for helping us improve our server by reporting this bug! Please fill out the form below with as much detail as possible.
  - type: checkboxes
    attributes:
      label: Existing Issue Check
      description: Have you checked if there's already an existing issue for this bug?
      options:
        - label: Yes, I've checked existing issues
          required: true
  - type: textarea
    id: desc
    attributes:
      label: Description
      description: Please provide a detailed description of the issue you are facing.
      placeholder: "Enter your description here..."
    validations:
      required: true
  - type: textarea
    id: expected
    attributes:
      label: Expected Behavior
      description: What behavior did you expect to see?
      placeholder: "Describe the expected behavior..."
    validations:
      required: true
  - type: textarea
    id: repro
    attributes:
      label: Steps to Reproduce
      description: Please provide step-by-step instructions on how to reproduce the issue.
      placeholder: |
        1. Run this command...
        2. Do this action...
        3. Press this key...
    validations:
      required: true
  - type: input
    id: texture
    attributes:
      label: Texture Packs
      description: If applicable, list any texture packs you are using (e.g., NVE).
      placeholder: "Enter texture packs used (if any)"
    validations:
      required: false
