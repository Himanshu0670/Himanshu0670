# Related UCs
- [Diagnosis & Medical History - Add](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-Add.md)(To do)
- [Diagnosis & Medical History - View&Edit](/../main/Webusecase/ClinicalFlow/Issue%20Assistive%20Device-View%26Remove.md)(To do)

## Test Procedure includes: Add, View & Edit Diagnosis & Medical History 

<details open>
   <summary><h2>1. Diagnosis & Medical History- Add ✅ ❌ </h2></summary>

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
   <summary><h2>2. Diagnosis & Medical History- View  ✅ ❌ </h2></summary>

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
2.01 |Select a patient from **Patient list** whose **Diagnosis & Medical History** is not recorded |User navigates to the **Patient landing** screen,`ADD` button is displayed on **Diagnosis & Medical History** card|| ✅ ❌
2.02 |Select a patient from **Patient list** whose **Diagnosis & Medical History** is recorded |User navigates to the **Patient landing** screen,`UPDATE` button is displayed on **Diagnosis & Medical History** card|| ✅ ❌
2.03 |Click on the `UPDATE` button on **Diagnosis & Medical History** card|User navigates to the **Diagnosis & Medical History** view screen || ✅ ❌
2.04 |Verify the details on the view screen of **Diagnosis & Medical History** card |Screen display following items: 🔙 button, Diagnosis & Medical History <date(dd month,yyyy) of creation/last update>, **General Medical Condition,Disability Type and Onset of Disability cards** with answers which was added during the Add/last update|| ✅ ❌
2.05 |Click on `EDIT` button of **General Medical Condition** card|User navigates to the **General Medical Condition** edit screen|| ✅ ❌
2.06 |Click on `EDIT` button of **Disability Type** card|User navigates to the **Disability Type** edit screen|| ✅ ❌
2.07 |Click on `EDIT` button of **Onset of Disability** card|User navigates to the **Onset of Disability** edit screen|| ✅ ❌
2.08 |Click on the 🔙 button on view screen |User navigates to the **Patient landing** screen|| ✅ ❌


</details>

<details open>
   <summary><h2>3. Diagnosis & Medical History- Edit  ✅ ❌ </h2></summary>

### Pre-condition
This section is executed when **Diagnosis & Medical History** is recorded of a patient.To record Diagnosis & Medical History of a patient execute (TP 1.01 to 1.49)

## Actor 
- **Healthcare Provider**
- **Admin**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
3.01 |Select a patient from **Patient list** whose **Diagnosis & Medical History** is not recorded |User navigates to the **Patient landing** screen,`ADD` button is displayed on **Diagnosis & Medical History** card|| ✅ ❌
3.02 |Select a patient from **Patient list** whose **Diagnosis & Medical History** is recorded |User navigates to the **Patient landing** screen,`UPDATE` button is displayed on **Diagnosis & Medical History** card|| ✅ ❌
3.03 |Click on the `UPDATE` button on **Diagnosis & Medical History** card|User navigates to the **Diagnosis & Medical History** view screen || ✅ ❌
3.04 |Click on `EDIT` button of **General Medical Condition** card|User navigates to the **General Medical Condition** edit screen|| ✅ ❌
3.05 |Click on `EDIT` button of **Disability Type** card|User navigates to the **Disability Type** edit screen|| ✅ ❌
3.06 |Click on `EDIT` button of **Onset of Disability** card|User navigates to the **Onset of Disability** edit screen|| ✅ ❌



</details>
