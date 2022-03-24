# Data Virtualization
## Summary
### Issue
Describe why we need a tool in this domain, any context necessary. 
Example: We need to store secrets, such as passwords, private keys, and tokens.

If there are sub-domains that might require unique tools, describe those here as well.
Example: Secrets used by an individual vs secrets used by a system would have different solutions.

### Decision
List the selected solution, including a link to the official website. 
If there are multiple solutions, describe a precise scenario where the reader should apply that solution so that they may make an informed choice.
Example: [Bitwarden](https://go.bitwarden.com/password-management-for-business-teams-organizations/?utm_source=google&utm_medium=cpc&utm_campaign=AW_USCA_NU_CL_Bitwarden_en_GSN_DTMB_Brand_KW:Brand_Exact&utm_content=475928674547&utm_term=bitwarden&gclid=CjwKCAjwzaSLBhBJEiwAJSRoktT5RvR71MB2vDwV2wzKL5Jo5ViWtgN-2Y9qC6wANnKngqeRQ5r3jRoCM1AQAvD_BwE) for user-oriented secrets, [Vault by Hashicorp](https://www.vaultproject.io/) for system-oriented secrets

### Status
Select one: 
- Hold: if an assessment is not currently in progress and no decision has been made yet.
- Assess: if an assessment of the products is currently underway.
- Trial: if a trial of a product is currently underway.
- Use: if a decision has been made and adopted by the enterprise.

Indicate how open you are to reviewing new options in this space going forward.

## Details
### Requirements
List out requirements for the tools, any assumptions and/or constraints. Example: individual secret management must be capable of auto-filling the username/password into website forms.
### Considered Solutions
List out the options/products that are available in this space and will be / have been assessed. Example: Bitwarden, LastPass, 1Password.
You do not need to complete full trials with each position listed. If they were in any way considered, list them here. Then, in the below notes section, describe the level of investigation you committed to the option and why.
### Rationale
Describe key reasons behind the decision, either for one option or against the others. Example: Bitwarden is open source and has a strong security track-record.
### Consequences
Describe any implications of the decision, and any drawbacks. Example: LastPass will be decommissioned in favor of BitWarden and we will need to provide a migration path.

## Related
Describe any knock-on decisions that arose as part of this assessment. Provide links to those decision documents wherever possible.
You may also consider documenting related requirements, artifacts, or principles here.

## Notes
Provide evaluation notes for each option that was evaluated: features, why it was considered, how it was evaluated and to what extent, conclusions.

To get user feedback on various solutions, we recommend the following polling framework:
Create a Google Form with scoring options 1-5: 
1. This would be a terrible mistake
2. This might work, but there are some issues to be addressed first
3. This is not my first choice, but I understand the appeal and would be willing to go along with a decision to use it
4. This is the best option from what we have available
5. This is the best solution ever

If someone provides a score of 2 or lower, ask them to document their specific concerns and see if they can be addressed. If they cannot be addressed, these must be captured in the Consequences section above. Find a solution where the majority of the participants rate it a 3 or higher.