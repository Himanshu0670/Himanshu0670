# Related UCs
- [DisabilityAssessment-Add](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-Add.md)
- [DisabilityAssessment-View&Edit](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-View%26Remove.md)

## Test Procedure includes: Add, Edit & View disability assessment 

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
1.18 |Try to select more than one radio button for a question |Only one radio button for a question is selected|| ✅ ❌
1.19 |Answer all the mandatory questions,click on the `SAVE` button|Data is saved,user navigates to the **Patient landing** screen with a success toast message: "**Disability assessment data saved**"|| ✅ ❌
</details>

<details open>
   <summary><h2>2. DisabilityAssessment- Edit  ✅ ❌ </h2></summary>

### Pre-condition
This section is executed when at least one **`WG-SS` disability assessment** is done of a patient.To do a disability assessment a patient execute (TP 1.01 to 1.19)

## Actor 
- **Health Care Provider**
- **Front Office Staff**
- **Field Worker**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
3.01 |Select a patient from **Patient list**|User navigates to the **Patient landing** screen|| ✅ ❌
3.02 |Click on the Disability assessment **<date(dd month,yyyy) of creation/last update>** card|User navigates to the **Disability assessment** view screen || ✅ ❌
3.03 |Check the **Disability assessment** view screen next day of disability assessment creation|`EDIT`button is not displayed on view screen || ✅ ❌
3.04 |Check the **Disability assessment** view screen same day of disability assessment creation/last update|`EDIT`button is displayed on view screen || ✅ ❌
3.05 |Click on the `EDIT` button|User navigates to the **Disability assessment** edit screen || ✅ ❌
3.06 |Verify the details on the edit screen |Screen display following items: 🔙 button, Disability assessment <date(dd month,yyyy) of creation/last update>,Pre-filled six mandatory questions which was added during the Add/last update & `SAVE` (button in enabled state)|| ✅ ❌
3.07 |Select the “**No difficulty**” radio button for all questions|“**No difficulty**” radio button is selected|| ✅ ❌
3.08 |Select the “**Some difficulty**” radio button for all questions|“**Some difficulty**” radio button is selected|| ✅ ❌
3.09 |Select the “**A lot of difficulty**” radio button for all questions|“**A lot of difficulty**” radio button is selected|| ✅ ❌
3.10 |Select the “**Cannot do at all**” radio button for all questions|“**Cannot do at all**” radio button is selected|| ✅ ❌
3.11 |Update answer for question **Do you have difficulty seeing, even if wearing glasses?*** by selecting any other radio button|Radio button is selected|| ✅ ❌
3.12 |Update answer for question **Do you have difficulty hearing, even if using a hearing aid(s)?*** by selecting any other radio button|Radio button is selected|| ✅ ❌
3.13 |Update answer for question **Do you have difficulty walking or climbing steps?*** by selecting any other radio button|Radio button is selected|| ✅ ❌
3.14 |Update answer for question **Do you have difficulty remembering or concentrating?*** by selecting any other radio button|Radio button is selected|| ✅ ❌
3.15 |Update answer for question **Do you have difficulty with self-care, such as washing all over or dressing?*** by selecting any other radio button|Radio button is selected|| ✅ ❌
3.16 |Update answer for question **Using your usual language, do you have difficulty communicating, for example understanding or being understood?*** by selecting any other radio button|Radio button is selected|| ✅ ❌
3.17 |Select any one radio button for all the mandatory questions|Radio button is selected|| ✅ ❌
3.18 |Try to select more than one radio button for a question |Only one radio button for a question is selected|| ✅ ❌
3.19 |Try to deselect radio button of a question |Selected radio button cannot be deselect|| ✅ ❌
3.20 |Update all the mandatory questions,click on the `SAVE` button|Data is saved,user navigates to the **Patient landing** screen with a success toast message: "**Disability assessment data updated**"|| ✅ ❌
3.21 |Do not update questions,click on the `SAVE` button|Data is saved,user navigates to the **Patient landing** screen with a success toast message: "**Disability assessment data updated**"|| ✅ ❌


