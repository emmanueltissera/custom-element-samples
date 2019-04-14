# Components element

In Kentico Cloud there is linked items element as well as linked items as a part of the rich text. Then there are components as a part of the rich text, but there are components missing as a stand-alone element so editors can't create as many components as they need with no related items created.

You can test it by configuring https://emmanueltissera.github.io/custom-element-samples/IconSelector/index.html url for your custom element.

You can provide an array of icons to be displayed with their source files, labels and values.

![screenshot](https://lh3.googleusercontent.com/0zFxpQlplzKOVyNDkmRP4vtiQ1fOrlBMJzJToEYK18FpaJ9kCwuFg30CkkbDgRd6TWSlzVZeXfhzh4Fn71mDy1hjmGspP1OWkgLDzHwd9ObcYeWie7hUI2P7uHj5_wSbyYT8gXVyBA=w822-h353-no)

This outputs to:
```text
projectManager
```

## Configuration

The main `controlLabel` parameter is used to show the text on the dropdown.

Your have to configure `controlLabel` and `options` parameters. There should be at least more than one option for this to work.

Following {JSON} parameters show five options specified:

```json
{
  "controlLabel": "Please select an OSA icon",
  "options": [
    {
      "label": "Firewall",
      "value": "firewall",
      "icon": "https://emmanueltissera.github.io/custom-element-samples/IconSelector/samples/osa_firewall.svg"
    },
    {
      "label": "Home",
      "value": "home",
      "icon": "https://emmanueltissera.github.io/custom-element-samples/IconSelector/samples/osa_home.svg"
    },
    {
      "label": "Architect",
      "value": "architect",
      "icon": "https://emmanueltissera.github.io/custom-element-samples/IconSelector/samples/osa_user_green_architect.svg"
    },
    {
      "label": "Project Manager",
      "value": "projectManager",
      "icon": "https://emmanueltissera.github.io/custom-element-samples/IconSelector/samples/osa_user_green_project_manager.svg"
    },
    {
      "label": "Security Specialist",
      "value": "security-specialist",
      "icon": "https://emmanueltissera.github.io/custom-element-samples/IconSelector/samples/osa_user_blue_security_specialist.svg"
    }
  ]
}
```

![screenshot](https://lh3.googleusercontent.com/kQc5uQEul8StZNRCLAtZ6XC2eT8PLx0qc9KlZC2q4UwoXj3sXoII5V0z5r3mvSTVaKseda_DvfhoKqkhAxrhoNeO8iYKD8Fn-0r94IX7ewRd8XzeggFMEhOj8rrOydgYAlVgCOtCHQ=w1013-h1028-no)