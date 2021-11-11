# Draw IT

## Overview

Draw IBM2 IT Architecture Diagrams.

Input: RIAS or YAML

Output: draw.io

Note: YAML can be user-created.

## RIAS Steps

1. Create API Key if not already created:
- Login to [IBM Cloud Portal](https://cloud.ibm.com/).
- Go to **Manage** and select **Access (IAM)**.
- Go to **API keys** and select **Create an IBM Cloud API key**.
- Copy the API Key.
2. Convert RIAS to drawio file(s):
- Start **Draw IT** application.
- Copy API Key into **API Key** field.
- (Optional) Copy Account ID into **Account ID** field.
- Leave **YAML File** blank.
- Use default directory or click **Select Directory** to change directory.
- Select **Region**.
- Select **Detail Level**.
- Select **Diagram Type**.
- Select **File Organization**.
- Select **Generate**.
3. View in drawio:
- Install and start [IBM v2 drawio desktop](https://github.com/ibm-cloud-architecture/ibm-cloud-stencils/releases) application.
- Click **Open Existing Diagram** and browse to draw.io file.

## Features

Groups:
| Group | Status | 
| --- | --- |
| Cloud | Implemented |
| Region | Implemented |
| Zone | Implemented |
| VPC | Implemented |
| Subnet | Implemented |
| Public Network | Implemented |
| Enterprise Network | Implemented |

Icons:
| Icon | Type | Status | 
| --- | --- | -- |
| User | Actor | Implemented |
| Instance | Collapsed Node | Implemented |
| Instance | Expanded Node | Implemented |
| Public ALB | Collapsed Node | Implemented |
| Public Gateway | Collapsed Node | Implemented |
| VPN Gateway | Collapsed Node | Disabled |

Arrows:
| Arrow | Type | Status | 
| --- | --- | -- |
| Floating IP | Double Arrow | Implemented |
| Public ALB | Double Arrow | Implemented |
| Public Gateway | Single Arrow | Implemented |

Notes:
1. For RIAS on your account, all VPC functionality can be accessed.
