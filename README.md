# Draw IT

## Overview

Draw IBM2 IT Architecture Diagrams.

Input: RIAS or YAML

Output: draw.io

Note: YAML can be from either Ops Dashboard or user-created.

Latest release: [DrawIT-0.1.18](releases.md)

## RIAS Steps

1. Create API Key if not already created:
- Login to [IBM Cloud Portal](https://cloud.ibm.com/).
- Go to **Manage** and select **Access (IAM)**.
- Go to **API keys** and select **Create an IBM Cloud API key**.
- Copy the API Key.
2. (Optional) Get Account ID:
- From [IMS Portal](https://internal.softlayer.com/User/dashboard), enter customer name in **Search** on **Customer Name**, select the desired customer account in the search results, click on the BlueMix symbol in upper right, and copy the IBM Cloud Account ID.
- From [VPC Operations Dashboard](https://opsdashboard.w3.cloud.ibm.com/ops/landing), enter customer name in **Search**, select the desired customer account in the search results, and copy the IBM Cloud Account ID.
3. Convert RIAS to drawio file(s):
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
4. Set layout and view in drawio:
- Install and start [IBM v2 drawio desktop](https://github.com/ibm-cloud-architecture/ibm-cloud-stencils/releases) application.
- Click **Open Existing Diagram** and browse to draw.io file.

## Ops Dashboard Steps

1. Retrieve Account YAML:
- Login to [VPC Operations Dashboard](https://opsdashboard.w3.cloud.ibm.com/ops/landing).
- Enter customer name in **Search**.
- Select an account.
- Select **Export Account**.
2. Convert YAML to drawio file(s):
- Install and start [Draw IT](https://github.ibm.com/acs-sa/DrawIT) application.
- Click **Select YAML** and browse to YAML file.
- Use default directory or click **Select Directory** to change directory.
- Select **Region**.
- Select **Detail Level**.
- Select **Diagram Type**.
- Select **File Organization**.
- Select **Generate**.
3. Set layout and view in drawio:
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
1. For Ops Dashboard, secure access is required to export YAML for your own account and other accounts.
2. For RIAS on your account, all VPC functionality can be accessed.
3. For RIAS on other accounts, base VPC functionality can be accessed but Load Balancer and VPN Gateway require whitelisting. 
