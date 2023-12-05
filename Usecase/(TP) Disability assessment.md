# Related UCs
- [DisabilityAssessment-Add](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-Add.md)
- [DisabilityAssessment-View&Edit](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-View%26Remove.md)

## Test Procedure includes: Add, Remove & View issue assistive devices

<details open>
   <summary><h2>1. DisabilityAssessment- Add  ✅ ❌ </h2></summary>

### Pre-condition
- This section is executed when user login in to the system & at least one patient should be registered.

## Actor 
- **Health Care Provider**
- **Front Office Staff**
- **Field Worker**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
1.01 |Select a patient from **Patient list**|User navigates to the **Patient landing** screen|| ✅ ❌
1.02 |Click on the `START` button of`“Disability Assessment” on the **Patient landing** screen|User navigates to the “**Disability Assessment**” screen|| ✅ ❌
1.03 |Verify the details on the screen|Screen display following items in empty state:❎ button, Disability assessment <selected patient name(first+middle+last)>,`Gender/Age`,Six mandatory questions mentioned in Vanuatu MDR: [workflow](https://docs.google.com/document/d/1RqBZYZhrnFEiOvU8gxUqofLYwvitQAlETRXzwW4Xtr0/edit#heading=h.ow5vkgl9hyc2) & `Save` (button in disabled state)|| ✅ ❌
1.04 |Click on the ❎ button|User navigates to the **Patient landing** screen|| ✅ ❌
1.05 |Answer all the mandatory questions,check the `SAVE` button|`SAVE` button is enabled|| ✅ ❌
1.06 |Do not answer all the mandatory questions,check the `SAVE` button|`SAVE` button is disabled|| ✅ ❌
1.07 |Select the “**No difficulty**” radio button for all questions|“**No difficulty**” radio button is selected|| ✅ ❌
1.08 |Select the “**Some difficulty**” radio button for all questions|“**Some difficulty**” radio button is selected|| ✅ ❌
1.09 |Select the “**A lot of difficulty**” radio button for all questions|“**A lot of difficulty**” radio button is selected|| ✅ ❌
1.10 |Select the “**Cannot do at all**” radio button for all questions|“**Cannot do at all**” radio button is selected|| ✅ ❌
1.11 |Select any one radio button for question **Do you have difficulty seeing, even if wearing glasses?***|Radio button is selected|| ✅ ❌
1.12 |Select any one radio button for question **Do you have difficulty hearing, even if using a hearing aid(s)?***|Radio button is selected|| ✅ ❌
1.13 |Select any one radio button for question **Do you have difficulty walking or climbing steps?***|Radio button is selected|| ✅ ❌
1.14 |Select any one radio button for question **Do you have difficulty remembering or concentrating?***|Radio button is selected|| ✅ ❌
1.15 |Select any one radio button for question **Do you have difficulty with self-care, such as washing all over or dressing?***|Radio button is selected|| ✅ ❌
1.16 |Select any one radio button for question **Using your usual language, do you have difficulty communicating, for example understanding or being understood?***|Radio button is selected|| ✅ ❌
1.17 |Select any one radio button for all the mandatory questions|Radio button is selected|| ✅ ❌
1.18 |Try to select more than one radio button for a question |Only one radio button is selected|| ✅ ❌
1.19 |Answer all the mandatory questions,click on the `SAVE` button|Data is saved,user navigates to the **Patient landing** screen with a success toast message: "**Disability assessment data saved**"|| ✅ ❌

</details>
