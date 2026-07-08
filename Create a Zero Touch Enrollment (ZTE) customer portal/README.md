# Create a Zero Touch Enrollment (ZTE) customer portal

## Requirements:   
| What You Need                        | Status                                                                      |
| ------------------------------------ | --------------------------------------------------------------------------- |
| Custom Google domain (not Gmail)     | ✅ Required                                                                  |
| Authorized reseller or Google direct | ✅ Required                                                                  |
| Compatible Android 9+ devices        | ✅ Required                                                                  |
| Super Admin access on domain         | ✅ Required                                                                  |
| Separate MDM (e.g., Intune, WorkSpace ONE)     | ⚠️ Not required for portal creation, but needed for actual device management |


---
---

## A Google Workspace or Cloud Identity Domain

| Requirement             | Details                                                                                                                            |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| **Domain type**         | Google Workspace (paid) or Cloud Identity Free                                                                                     |
| **Why needed**          | The Zero Touch customer account is tied to a Google organization. You sign into the portal with an admin account from this domain. |
| **Gmail.com addresses** | ❌ Not supported — you need a custom domain (e.g., `admin@yourcompany.com`)                                                         |

## An Authorized Zero Touch Reseller or Direct Google Relationship
| Path                        | How It Works                                                                                                                                                    |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Via authorized reseller** | Most common. Purchase Android devices from a reseller who is a Google Zero Touch partner. They create the customer account association and upload your devices. |
| **Direct with Google**      | Large enterprises buying devices directly from Google can get set up without a reseller intermediary.                                                           |

## Compatible Devices

| Requirement              | Details                                                                                             |
| ------------------------ | --------------------------------------------------------------------------------------------------- |
| **Android version**      | Android 9.0 (Pie) or higher                                                                         |
| **Manufacturer support** | Device OEM must participate in Google's Zero Touch program                                          |
| **Device origin**        | Must be purchased through an authorized channel — retail/consumer devices typically cannot be added |

## Super Admin Permissions

| Requirement               | Details                                                                                                                   |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Super Admin**           | On your Google Workspace/Cloud Identity domain, you need Super Admin rights to access and configure the Zero Touch portal |
| **Zero Touch Admin role** | Once the account is set up, you can delegate Zero Touch-specific admin roles to other users                               |

## Setup Process (High Level)
1. **Purchase devices** through an authorized Zero Touch reseller (or Google directly)
2. **Provide your Google Workspace domain** to the reseller during purchase
3. **Reseller uploads device IMEIs** and associates them with your domain
4. **Google sends an invitation email** to your domain's Super Admin
5. **Accept the invitation** and sign into https://enterprise.google.com/android/zero-touch/customers/
6. **Create configurations** and assign them to your device batches


## If You Already Have a Domain
If the customer organization already uses Google Workspace or Cloud Identity, you can likely use the existing domain.    
⚠️ The key step is ensuring the device reseller knows to associate purchases with that domain.

## Cost
| Component                         | Cost                                                        |
| --------------------------------- | ----------------------------------------------------------- |
| Google Workspace / Cloud Identity | Standard subscription fees (Cloud Identity Free is \$0)     |
| Zero Touch service itself         | **Free** — Google does not charge for Zero Touch enrollment |
| Compatible devices                | Regular device cost (no premium for Zero Touch capability)  |

