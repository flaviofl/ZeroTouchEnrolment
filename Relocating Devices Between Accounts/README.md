# Relocating Devices Between Accounts

Devices can be moved from one Zero Touch customer account to another, but the process has specific rules:


| Action                           | Who Can Do It                   | Details                                                                                                                             |
| -------------------------------- | ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **Unclaim from current account** | Customer admin (source account) | In the ZTE customer portal, select the device → **Unclaim**. This removes it from your account and makes it available for reassignment. |
| **Claim to new account**         | Reseller or Google              | The target account's reseller must upload the IMEI to the new account, or Google support can assist for direct customers.           |

## Important Caveats
- **You cannot directly transfer a device** from Account A to Account B yourself — you can only unclaim it. The receiving account must then claim it.
- **The device must not be actively enrolled** — It's best to factory reset and unenroll before unclaiming.
- **Reseller involvement is usually required** for the receiving account to claim the device, unless both accounts are under the same Google direct-billing arrangement.
- Some resellers charge a fee for re-uploading devices to a different account.

## Workflow for Moving Devices
1. **Factory reset** the device (if already enrolled)
2. **Unclaim the device** from the source Zero Touch account
3. Provide the **IMEI list** to the reseller/admin of the target account
4. **Reseller uploads IMEIs** to the target account
5. **Assign configuration** in the target account (Customer Portal)
6. Device enrolls into the new MDM/environment on next setup