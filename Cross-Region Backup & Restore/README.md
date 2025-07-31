Project Title

Cross-Region Backup & Restore of Azure VM using Azure Recovery Services Vault


📌 Objective
This project demonstrates how to configure backup for an Azure VM using Recovery Services Vault (RSV) and perform a cross-region restore to a different Azure region, ensuring disaster recovery and business continuity.


🧱 Tech Stack

✅ Azure VM (Windows/Linux)

✅ Recovery Services Vault

✅ Backup Policy

✅ Azure Storage Account (ZRS)

✅ Cross-Region Restore (CRR)



📍 Regions Used

Primary Region: East US

Secondary (Recovery) Region: West US


🛠️ Key Steps Performed
1. Created Recovery Services Vault in East US

2. Enabled Cross-Region Restore (CRR)

3. Configured Backup for VM using a new backup policy

4. Took On-Demand Backup to trigger recovery point

5. Created ZRS Storage Account in West US (for restore staging)

6. Restored VM to Secondary Region with new name: CRR-VM-DR

7. Tested VM Connectivity using Public IP + Username/Password

8. Disabled Soft Delete to clean up restore points

9. Deleted all Resources after validation


🔁 Cross-Region Restore Demo Diagram



✅ Outcome
Successfully demonstrated end-to-end VM backup and cross-region restore

Validated the restored VM was fully operational in West US

Ensured backup compliance, disaster recovery readiness, and clean deletion of resources after testing

