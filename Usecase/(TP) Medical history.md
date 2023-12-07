# Related UCs
- [Diagnosis & Medical History - Add](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-Add.md)(To do)
- [Diagnosis & Medical History - View&Edit](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-View%26Remove.md)(To do)

## Test Procedure includes: Add, View & Edit Diagnosis & Medical History 

<details open>
   <summary><h2>1. Diagnosis & Medical History - Add ✅ ❌ </h2></summary>

### Pre-condition
- This section is executed when a Disability assessment is recorded of a patient.

## Actor 
- **Healthcare Provider**
- **Admin**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
1.01 |Select a patient from **Patient list**|User navigates to the **Patient landing** screen|| ✅ ❌
1.02 |Check when Disability assessment is not recorded of a patient|Diagnosis & Medical History card is not displayed on **Patient landing** screen || ✅ ❌
1.03 |Check when Disability assessment is recorded of a patient|Diagnosis & Medical History card is displayed on **Patient landing** screen || ✅ ❌
1.04 |Click on the `ADD` button on Diagnosis & Medical History card|User navigates to the Diagnosis & Medical History `General Medical Conditions` sub-section screen|| ✅ ❌
1.05 |Verify the details on the `General Medical Conditions` screen|Screen display following items in empty state: ❎ close button, Diagnosis & medical history of <selected patient name(first+middle+last)>,Gender/Age General Medical Conditions checkbox options[Link](https://docs.google.com/document/d/1RqBZYZhrnFEiOvU8gxUqofLYwvitQAlETRXzwW4Xtr0/edit#heading=h.kf6buc86qsnl) & `NEXT` (button in enabled state).|| ✅ ❌
1.06 |Click on the ❎ close button|User navigates to the **Patient landing** screen|| ✅ ❌
1.07 |Do not select any checkbox option on `General Medical Conditions` screen,check the `NEXT` button|`NEXT` button is enabled|| ✅ ❌
1.08 |Select only one checkbox option on `General Medical Conditions` screen - `Diabetes`|Checkbox option is selected|| ✅ ❌
1.09 |Select more than one checkbox options on `General Medical Conditions` screen - `Hypertension`,`Asthma`,`Cancer`|Checkbox options is selected|| ✅ ❌
1.10 |Deslect `Asthma` checkbox option|Option is deselected|| ✅ ❌
1.11 |Select `Other` checkbox option,check the screen|`Please specify*` mandatory textfield is displayed|| ✅ ❌
1.12 |After selecting `Other`checkbox option,do not enter value in mandatory textfield|`NEXT` button is disabled|| ✅ ❌
1.13 |Enter -`A while backed I needed to count the amount of letters that a piece of text in an email template had (to avoid passing any character limits). Unfortunately, I could not think of a quick way to so on my` in **Please specify*** textfield|The last character `y` is truncated|| ✅ ❌
1.14 |Select `Old Age`checkbox option on `General Medical Conditions` screen,click on `NEXT` button|User navigates to the Diagnosis & Medical History `Disability Type` sub-section screen|| ✅ ❌
1.15 |Verify the details on the `Disability Type` screen|Screen display following items in empty state: ❎ close button, Diagnosis & medical history of <selected patient name(first+middle+last)>,Gender/Age Disability Type checkbox options[Link](https://docs.google.com/document/d/1RqBZYZhrnFEiOvU8gxUqofLYwvitQAlETRXzwW4Xtr0/edit),`BACK` & `NEXT`(button in enabled state).|| ✅ ❌
1.16 |Click on `BACK` button on `Disability Type` screen|User navigates to the `General Medical Conditions` screen || ✅ ❌
1.17 |Select “Physical Impairment” checkbox |“Physical Impairment” is selected,Sub-options is triggered|| ✅ ❌
1.18 |Select “Visual Impairment” checkbox |“Visual Impairment” is selected,Sub-options is triggered|| ✅ ❌
1.19 |Select “Hearing Impairment” checkbox |“Hearing Impairment” is selected,Sub-options is triggered|| ✅ ❌
1.20 |Select “Communication Impairment” checkbox |“Communication Impairment” is selected,Sub-options is triggered|| ✅ ❌
1.21 |Select “Self-care Impairment” checkbox |“Self-care Impairment” is selected,Sub-options is triggered|| ✅ ❌
1.22 |Select “Other Impairment” checkbox |“Other Impairment” is selected,`Please specify*` mandatory textfield is triggered|| ✅ ❌
1.23 |Select `Other` checkbox option on “Physical Impairment” sub-options|`Other` option is selected,`Please specify*` mandatory textfield is triggered|| ✅ ❌
1.24 |Select `Other` checkbox option on “Visual Impairment” sub-options|`Other` option is selected,`Please specify*` mandatory textfield is triggered|| ✅ ❌
1.25 |Select `Other` checkbox option on “Hearing Impairment” sub-options|`Other` option is selected,`Please specify*` mandatory textfield is triggered|| ✅ ❌
1.26 |Select `Other` checkbox option on “Communication Impairment” sub-options|`Other` option is selected,`Please specify*` mandatory textfield is triggered|| ✅ ❌
1.27 |Select `Other` checkbox option on “Self-care Impairment” sub-options|`Other` option is selected,`Please specify*` mandatory textfield is triggered|| ✅ ❌
1.28 |Select any other checkbox option except `Other`on any sub-options|No further question is appeared || ✅ ❌
1.29 |Do not enter value in `Please specify*`mandatory textfield |`NEXT` button is disabled || ✅ ❌
1.30 |Enter -`A while backed I needed to count the amount of letters that a piece of text in an email template had (to avoid passing any character limits). Unfortunately, I could not think of a quick way to so on my` in **Please specify*** textfield|The last character `y` is truncated|| ✅ ❌
1.31 |Do not select any checkbox option on `Disability Type` screen |`NEXT` button is enabled || ✅ ❌
1.32 |Select any checkbox option on `Disability Type` screen |`NEXT` button is disabled until at least one sub-option is not selected except (Other) option|| ✅ ❌
1.33 |Select more than one sub-option checkbox for any "Impairment" option except("Other Impairment") on `Disability Type` screen|`NEXT` button is enabled || ✅ ❌
1.34 |Select “`Visual Impairment`” checkbox & "`Use glasses`" sub-options,click on the `NEXT` button |User navigates to the Diagnosis & Medical History `Onset of Disability` sub-section screen|| ✅ ❌
1.35 |Verify the details on the `Onset of Disability` screen|Screen display following items in empty state: ❎ close button, Diagnosis & medical history of <selected patient name(first+middle+last)>,Gender/Age Onset of Disability questions [Link](https://docs.google.com/document/d/1RqBZYZhrnFEiOvU8gxUqofLYwvitQAlETRXzwW4Xtr0/edit#heading=h.gdokhetj78vk),`BACK` & `SAVE`(button in enabled state).|| ✅ ❌
1.36 |Click on `BACK` button on `Onset of Disability` screen|User navigates to the `Disability Type` screen|| ✅ ❌
1.37 |Click on ❎ button on `Onset of Disability` screen|User navigates to the **Patient landing** screen|| ✅ ❌
1.38 |Do not answer any questions |`SAVE` button is enabled || ✅ ❌
1.39 |Select `Yes` radio button of Question **“Was the patient born prematurely?”**|Radio button is selected|| ✅ ❌
1.40 |Select `No`  radio button of Question **“Was the patient born prematurely?”**|Radio button is selected|| ✅ ❌
1.41 |Select `Yes` radio button of Question **“Was the patient born with a disability?”**|Radio button is selected|| ✅ ❌
1.42 |Select `No`  radio button of Question **“Was the patient born with a disability?”**|Radio button is selected|| ✅ ❌
1.43 |Select `Yes` radio button of Question **“Is old age the cause of the disability?”**|Radio button is selected|| ✅ ❌
1.44 |Select `No`  radio button of Question **“Is old age the cause of the disability?”**|Radio button is selected|| ✅ ❌
1.45 |Try to select both radio buttons|Only one radio button is selected at a time|| ✅ ❌
1.46 |Select `Yes` in all questions|`Yes` is selected in all questions || ✅ ❌
1.47 |Select `No` in all questions|`No` is selected in all questions || ✅ ❌
1.48 |Do not fill any data in any sub-section of **Diagnosis & medical history**,click on `SAVE` button|`No data recorded` toast message is displayed|| ✅ ❌
1.49 |Select `Yes` radio button of Question **“Was the patient born prematurely?”**,click on `SAVE` button|Data is saved, user navigates to the **Patient landing** screen with a success toast message -`Diagnosis & medical history data saved`|| ✅ ❌

</details>

<details open>
   <summary><h2>2. Diagnosis & Medical History - View  ✅ ❌ </h2></summary>

### Pre-condition
This section is executed when **Diagnosis & Medical History** is recorded of a patient.To record Diagnosis & Medical History of a patient execute (TP 1.01 to 1.49)

## Actor 

- **Front Office Staff** (👁️)
- **Health Care Provider**(👁️)
- **Field Worker**(👁️)
- **Admin** (👁️)
- **Analyst** (👁️)
- **Device Issuer**(👁️)

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
2.01 |Select a patient from **Patient list** whose **Diagnosis & Medical History** is recorded |User navigates to the **Patient landing** screen,`UPDATE` button is displayed on **Diagnosis & Medical History** card|| ✅ ❌
2.02 |Select a patient from **Patient list** whose **Diagnosis & Medical History** is not recorded |User navigates to the **Patient landing** screen,`ADD` button is displayed on **Diagnosis & Medical History** card|| ✅ ❌
2.03 |Click on the `UPDATE` button on **Diagnosis & Medical History** card|User navigates to the **Diagnosis & Medical History** view screen || ✅ ❌
2.04 |Verify the details on the view screen of **Diagnosis & Medical History** card |Screen display following items: 🔙 button, Diagnosis & Medical History <date(dd month,yyyy) of creation/last update>, **General Medical Condition,Disability Type and Onset of Disability cards** with answers which was added during the Add/last update|| ✅ ❌
2.05 |Click on `EDIT` button of **General Medical Condition** card|User navigates to the **General Medical Condition** edit screen|| ✅ ❌
2.06 |Click on `EDIT` button of **Disability Type** card|User navigates to the **Disability Type** edit screen|| ✅ ❌
2.07 |Click on `EDIT` button of **Onset of Disability** card|User navigates to the **Onset of Disability** edit screen|| ✅ ❌
2.08 |Click on the 🔙 button on view screen |User navigates to the **Patient landing** screen|| ✅ ❌


</details>

<details open>
   <summary><h2>3. DisabilityAssessment- Edit  ✅ ❌ </h2></summary>

### Pre-condition
This section is executed when at least one **`WG-SS` disability assessment** is done of a patient.To do a disability assessment a patient execute (TP 1.01 to 1.19)

## Actor 
- **Front Office Staff**
- **Healthcare Provider**
- **Field Worker**
- **Admin**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
3.01 |Select a patient from **Patient list**|User navigates to the **Patient landing** screen|| ✅ ❌
3.02 |Click on the Disability assessment **<date(dd month,yyyy) of creation/last update>** card|User navigates to the **Disability assessment** view screen || ✅ ❌
3.03 |Check the **Disability assessment** view screen next day of disability assessment creation|`EDIT`button is not displayed on view screen || ✅ ❌
3.04 |Check the **Disability assessment** view screen same day of disability assessment creation/last update|`EDIT`button is displayed on view screen || ✅ ❌
3.05 |Click on the `EDIT` button|User navigates to the **Disability assessment** edit screen || ✅ ❌
3.06 |Verify the details on the edit screen |Screen display following items: 🔙 button, Disability assessment <date(dd month,yyyy) of creation/last update>,Pre-filled six mandatory questions which was answered during the Add/last update & `SAVE` (button in enabled state)|| ✅ ❌
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
</details>
