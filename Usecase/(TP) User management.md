# Related UCs
- [User List View](To do)
- [User- Add](To do)
- [User - View&Edit](To do)
- [Disable User](To do)

## Test Procedure includes: User list,Add,View & Edit User details. 

<details open>
   <summary><h2>1. User List View  ✅ ❌ </h2></summary>

### Pre-condition
- This section is executed when user login in to the system.

## Actor 
- **Admin**
- **Analyst** (👁️)

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
1.01 |Login successfully to the web|User navigates to the **User list view** screen|| ✅ ❌
1.02 |Verify the details on the User list screen|Screen display following items: User list,Filters by (Organization,Role,Status),Search field,`RESET FILTERS` & `ADD USER` button|| ✅ ❌
1.03 |Check the User list screen when no user is registered to the web|**No user registered yet, please click on ADD USER button to register a user.** text is displayed|| ✅ ❌
1.04 |Click on the top-right `Profile` icon|Dialog opens with user details|| ✅ ❌
1.05 |Click outside screen when profile details dialog opens |Profile details dialog closed|| ✅ ❌
1.06 |Check the user details on User list screen|User details is shown on the list view: Full name, Organization, Role, Mobile # & Status|| ✅ ❌
1.07 |Check the top-most record on the User list|Most recently added/updated user record is appears at the top of the list User list| ✅ ❌
1.08 |Check the filter options on User list screen|User can filter list by: `Organization``Role` & `Status`|| ✅ ❌
1.09 |Check the default value for `Organization` filter|`All` option is the default value for `Organization` filter|| ✅ ❌
1.10 |Click on the `Organization` filter field|Dropdown opens|| ✅ ❌
1.11 |Check the other dropdown option for `Organization` filter|List is fetched from the backend for `Organization` filter value|| ✅ ❌
1.12 |Select other dropdown option for `Organization` filter |Option is selected,User list is filtered accordingly|| ✅ ❌
1.13 |Select more than one dropdown option for `Organization` filter |Only one option is selected|| ✅ ❌
1.14 |Check the default value for `Role` filter|`All` option is the default value for `Role` filter|| ✅ ❌
1.15 |Click on the `Role` filter field|Dropdown opens|| ✅ ❌
1.16 |Check the other dropdown option for `Role` filter|Dropdown options: `All`, `Front office staff`, `Device issuer`, `Healthcare provider`, `Admin` & `Analyst` is displayed|| ✅ ❌
1.17 |Select `Admin` dropdown option for `Role` filter |Option is selected,User list is filtered accordingly|| ✅ ❌
1.18 |Select more than one dropdown option for `Role` filter |Only one option is selected|| ✅ ❌
1.19 |Check the default value for `Status` filter|`All` option is the default value for `Status` filter|| ✅ ❌
1.20 |Click on the `Status` filter field|Dropdown opens|| ✅ ❌
1.21 |Check the other dropdown option for `Status` filter|Dropdown options: `All`, `Active` & `Inactive`|| ✅ ❌
1.22 |Select `Active` dropdown option for `Status` filter |Option is selected,User list is filtered accordingly|| ✅ ❌
1.23 |Select more than one dropdown option for `Role` filter |Only one option is selected|| ✅ ❌
1.24 |Apply multiple filters - `Status` & `Role`,check the user list|User list is filtered according to the selected filters|| ✅ ❌
1.24 |Apply filter,check when no record found under filter criteria|`No results found` message is displayed|| ✅ ❌
1.25 |Click on the Search field|Field is clickable|| ✅ ❌
1.26 |Search user with `Full name` in User list|All the matched record is displayed|| ✅ ❌
1.27 |Search user with `Organization` in User list|All the matched record is displayed|| ✅ ❌
1.28 |Search user with `Role` in User list|All the matched record is displayed|| ✅ ❌
1.29 |Search user with `Mobile #` in User list|All the matched record is displayed|| ✅ ❌
1.30 |Search user with `Status` in User list|All the matched record is displayed|| ✅ ❌
1.31 |Click on search field,type `H` atleast one character - |Search functionality works,All the matched record is displayed|| ✅ ❌
1.29 |Click on search field,type `Device_$$`.Click on the ❎ button under search field |Entered value is removed from search field|| ✅ ❌
1.28 |Click on search field,type `Device_$$`,check when no record found in user list|`No results found` message is displayed|| ✅ ❌
1.29 |Check the `RESET FILTERS` button no fiters is applied on User list |`RESET FILTERS` button is disabled|| ✅ ❌
1.29 |Check the `RESET FILTERS` button when fiters is applied on User list |`RESET FILTERS` button is enabled|| ✅ ❌
1.28 |Click on search field,type `Device_$$`,check the `RESET FILTERS` button |`RESET FILTERS` button is enabled|| ✅ ❌




</details>

<details open>
   <summary><h2>2. DisabilityAssessment- View  ✅ ❌ </h2></summary>

### Pre-condition
This section is executed when at least one **`WG-SS` disability assessment** is done of a patient.To do a disability assessment a patient execute (TP 1.01 to 1.19)

## Actor 

- **Front Office Staff** (👁️)
- **Health Care Provider**(👁️)
- **Field Worker**(👁️)
- **Admin** (👁️)
- **Analyst** (👁️)
- **Device Issuer**(👁️)

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
2.01 |Select a patient from **Patient list**|User navigates to the **Patient landing** screen|| ✅ ❌
2.02 |Click on the Disability assessment **<date(dd month,yyyy) of creation/last update>** card|User navigates to the **Disability assessment** view screen || ✅ ❌
2.03 |Check the **Disability assessment** view screen next day of disability assessment creation|`EDIT`button is not displayed on view screen || ✅ ❌
2.04 |Check the **Disability assessment** view screen same day of disability assessment creation/last update|`EDIT`button is displayed on view screen || ✅ ❌
2.05 |Verify the details on the view screen next day of disability assessment creation |Screen display following items: 🔙 button, Disability assessment <date(dd month,yyyy) of creation/last update>,Pre-filled six mandatory questions which was answered during the Creation/last update|| ✅ ❌
2.06 |Click on the 🔙 button on view screen |User navigates to the **Patient landing** screen|| ✅ ❌


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
