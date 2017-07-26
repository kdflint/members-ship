New membership applications go into Applied status for 21 days. This is useful to plan for upcoming weeks. After 21 days, applications go to New status.

Weekly:

Run report "Grants Due for Approval". Important filters [CMS User:No; Membership Type:Grant; Membership Status:New]

For each application

     Reject
          Change Membership status to Rejected
          Send email with reason
               - Possibly invite to re-apply
               
     or Approve
          Apply Tag Approved
          
     or Ignore
     
Run report "Accepted Grants Due for Onboard". [CMS User:No; Membership Type:Grant; Tag:Approved] This report should output all the fields required by onboard.php

     Send grant award letter. 
          - Make sure to open up your Inbox to email from <address> with Subject line <whatever>

Onboard each Accept into NWM using onboard.php (Selenium???) This results in 

     set Nexus Activation Profile values
     apply tag Nexus Authorized
     
```
Still to solve - image
```

Run report "Onboarded Grants Due for Login". [CMS User:No; Membership Type:Grant; Tag:Approved; Tag:Authorized] This report should return the same number of memberships that you just Onboarded. This report should create a CSV file ready for import by Drupal Import module. Use the New Grantee configuration, which should

     Cause onboarding email to go out, with access instructions
