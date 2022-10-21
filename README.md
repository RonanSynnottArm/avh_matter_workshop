Simplify embedded software development and Continuous Integration (CI) at scale
---
## Welcome

Welcome to Arm DevSummit 2022. This workshop is to show you how to get started developing with [Matter](https://buildwithmatter.com) and [Arm Virtual Hardware](https://www.arm.com/products/development-tools/simulation/virtual-hardware), and to integrate into a CI/CD workflow.

This session is a hands-on workshop connecting to Arm Virtual Hardware in the cloud.

## Learning Objectives

By the end of this workshop, you will be able to:
* Instantiate Arm Virtual Hardware instances
* Build and run Matter examples on Arm Virtual Hardware
  * Demonstrate communication between two virtual hardware targets
* Use [GitHub Actions](https://github.com/features/actions) to manage ongoing development
  * Automate a CI/CD workflow

## Prerequisites

To participate in the workshops, attendees must have:

 - Personal computer with browser. Arm Virtual Hardware has been thoroughly tested with Chrome, Firefox, and Safari browsers.
 - User account for [Arm Virtual Hardware](https://avh.arm.com/)
 - User account for [GitHub](https://github.com/)

GitHub now requires a [Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) when pushing remote updates.

If you do not already have a token, you can create a new one via `Settings` > `Developer Settings` > `Personal access tokens`.

Ensure you have enabled the token to `Update GitHub Action workflows`.

You may wish to create a local scratchpad text file containing the below details (which will be unique to you), so that you can easily copy-and-paste from. These will be used frequently during this workshop.
```
YOUR_GITHUB_USERNAME
YOUR_PERSONAL_ACCESS_TOKEN
git config --global user.name "YOUR_GITHUB_USERNAME"
git config --global user.email YOUR_EMAIL_ADDRESS
```

## Sections

|      Type   | Content       |
| ---         | ---           |
| Section 1   | [Setup Arm Virtual Hardware instances](/1_setup.md) |
| Section 2   | [Build and run Matter examples on Arm Virtual Hardware](/2_build.md) |
| Section 3   | [Automate CI/CD workflow with a self-hosted runner](/3_cicdsh.md) |
| Section 4   | [Control Virtual Hardware with AVH API](/4_cicdapi.md) |

## References and Documentation

| Type          | Content             |
| ---           | ---                 |
| Website       | [Arm Virtual Hardware](https://avh.arm.com)      |
| Documentation | [AVH Product Overview](https://arm-software.github.io/AVH/main/overview/html/index.html) |
| Documentation | [Building Matter](https://github.com/project-chip/connectedhomeip/blob/master/docs/guides/BUILDING.md) |
| Blog          | [Welcome to the Virtual Raspberry Pi 4 running on AWS Graviton processors](https://dev.to/aws-builders/welcome-to-the-virtual-raspberry-pi-4-running-on-aws-graviton-processors-2o8e) |

## Thank you for attending

See the rest of the Arm DevSummit 2022 [program](https://devsummit.arm.com).

Learn more about [Arm in IoT](https://www.arm.com/solutions/iot).
