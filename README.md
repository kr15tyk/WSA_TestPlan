## Testplans_NDcPP

This repository uses a YAML script to generate custom NDcPPv3.0e conformant test plans. You can choose as many mandatory and/or selection-based SFRs as necessary to meet your test plan needs.

The generated test plans include the test cases a platform will need to pass in order to be certified under the [collaborative Protection Profile for Network Devices Version 3.0e (NDcPPv3.0e)](https://github.com/ND-iTC/Documents/blob/main/NDcPP_v3_0e.adoc).

These test cases are taken from the [Network Device Supporting Document Version 3.0e (NDSDv3.0e)](https://github.com/ND-iTC/Documents/blob/main/ND_Supporting_Document_3_0e.adoc) which defines the Evaluation Activities associated with the Security Functional Requirements (SFR) in the NDcPPv3.0e.

### Generate a Custom Test Plan

_You must be logged in to create a new repository._

1. Select **Use this template** button. 
2. Create a new repository with a unique repository name and make sure to not include all branches.
3. Check your repository permissions by going to Settings > Actions > General > WorkFlow permissions > select **Read and write permissions**, then Click **Save**.
4. [Create a branch](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/managing-branches#creating-a-branch). For example `sdwan_testplan_branch`
5. Delete any `.adoc` SFRs files you do not want included in your test plan. There are multiple ways to execute this step, (i.e., Git CLI, your local repository, in your browser).

* `NDv3.0e_mandatory_SFRs`
    ````
    - FAU_GEN_1.adoc
    - FAU_GEN_2.adoc
    - FAU_STG_EXT_1.adoc
    - FCS_CKM_1.adoc
    - FCS_CKM_2.adoc
    - FCS_CKM_4.adoc
    - FCS_COP_1_DataEncryption.adoc
    - FCS_COP_1_Hash.adoc
    - FCS_COP_1_KeyedHash.adoc
    - FCS_COP_1_SigGen.adoc
    - FCS_RBG_EXT_1.adoc
    - FIA_UIA_EXT_1.adoc
    - FMT_MOF_1_ManualUpdate.adoc
    - FMT_MTD_1_CoreData.adoc
    - FMT_SMF_1.adoc
    - FMT_SMR_2.adoc
    - FPT_SKP_EXT_1.adoc
    - FPT_STM_EXT_1.adoc
    - FPT_TST_EXT_1.adoc
    - FPT_TUD_EXT.1.adoc
    - FTA_SSL_3.adoc
    - FTA_SSL_4.adoc
    - FTA_TAB_1.adoc
    - FTP_ITC_1.adoc
    - FTP_TRP_1_Admin.adoc 
    ````

* `NDv3.0e_selection_based_SFRs`
    ````
    - FCS_DTLSC_EXT_1.adoc
    - FCS_DTLSS_EXT_1.adoc
    - FCS_HTTPS_EXT_1.adoc
    - FCS_IPSEC_EXT_1.adoc
    - FCS_NTP_EXT_1.adoc
    - FCS_TLSC_EXT_1.adoc
    - FCS_TLSS_EXT_1.adoc
    - FIA_AFL_1 .adoc
    - FIA_PMG_EXT_1.adoc
    - FIA_UAU_7.adoc
    - FIA_X509_EXT_1_Rev.adoc
    - FIA_X509_EXT_2.adoc
    - FIA_X509_EXT_3.adoc
    - FMT_MOF_1_AutoUpdate.adoc
    - FMT_MOF_1_Functions.adoc
    - FMT_MOF_1_Services.adoc
    - FMT_MTD_1_CryptoKeys.adoc
    - FPT_APW_EXT_1.adoc
    - FPT_TUD_EXT_2.adoc
    - FTA_SSL_EXT_1.adoc 
    ````

 * `PKG_SSHv1.0_SFRs`
    ````
    - FCS_SSH_EXT.1.adoc
    - FCS_SSHC_EXT.1.adoc
    - FCS_SSHS_EXT.1.adoc
    ````

6. From the Menu, select the **Actions** button.
7. Select **Combine Asciidoc, Convert to HTML, and Commit** workflow.
8. Select your new branch and then **Run workflow**. You can watch the workflow status as it runs. 
9. Return to your branch's page.
10. Download the `combined-testplan.adoc` and/or `testplan.html` documents.

_**NOTE:** It's recommended that you creating a new branch for each custom test plan you want to generate._
