# One Zero Touch Account

## What the Google Account Controls
The same Google account (Gmail or Google Workspace) can be used to integrate with multiple MDMs through Zero Touch, but with important distinctions:

| Element                         | What It Is                                                      | Can Be Shared?                                                            |
| ------------------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------- |
| **Zero Touch Customer Account** | Your organization's portal for managing devices                 | One account per customer tenant, but can have **multiple configurations** |
| **Configuration**               | A set of enrollment settings pointing to a specific MDM         | ✅ Multiple configurations per account                                     |
| **MDM Integration**             | The DPC extras / enrollment token that routes devices to an MDM | ✅ Different configs can point to different MDMs                           |


## Multiple MDMs
How Multiple MDMs Work in One Zero Touch Account?   
In your Zero Touch customer portal, you can create multiple configurations:   

    Account: admin@yourcompany.com   
    ├── Configuration A → MobiControl (DPC extras for SOTI MobiControl)   
    ├── Configuration B → Microsoft Intune (DPC extras for Intune)   
    ├── Configuration C → VMware Workspace ONE (DPC extras for WS1)   
    ├── Configuration D → Ivanti Neurons for MDM   
    └── Configuration E → Google Endpoint Management   

Then assign devices (or batches) to whichever configuration you need.

