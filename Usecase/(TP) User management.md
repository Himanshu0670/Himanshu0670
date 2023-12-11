# Related UCs
- [User List View](https://github.com/LatticeInnovations/vanuatu-mdr-main/blob/main/Web%20usecase/User_Management/UC_UserList.md)
- [User- Add](https://github.com/LatticeInnovations/vanuatu-mdr-main/blob/main/Web%20usecase/User_Management/UC_AddUser.md)
- [User - Edit](https://github.com/LatticeInnovations/vanuatu-mdr-main/blob/main/Web%20usecase/User_Management/UC_EditUser.md)
- [Disable User](https://github.com/LatticeInnovations/vanuatu-mdr-main/blob/main/Web%20usecase/User_Management/UC_DisableUser.md)

## Test Procedure includes: User list,Add,View & Edit user details. 

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
1.07 |Check the top-most record on the User list|Most recently added/updated user record is appears at the top of the list User list|| ✅ ❌
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
1.25 |Apply filter,check when no record found under filter criteria|`No results found` message is displayed|| ✅ ❌
1.26 |Click on the Search field|Field is clickable|| ✅ ❌
1.27 |Search user with `Full name` in User list|All the matched record is displayed|| ✅ ❌
1.28 |Search user with `Organization` in User list|All the matched record is displayed|| ✅ ❌
1.29 |Search user with `Role` in User list|All the matched record is displayed|| ✅ ❌
1.30 |Search user with `Mobile #` in User list|All the matched record is displayed|| ✅ ❌
1.31 |Search user with `Status` in User list|All the matched record is displayed|| ✅ ❌
1.32 |Click on search field,type `H` atleast one character - |Search functionality works,All the matched record is displayed|| ✅ ❌
1.33 |Click on search field,type `Device_$$`.Click on the ❎ button under search field |Entered value is removed from search field|| ✅ ❌
1.34 |Click on search field,type `Device_$$`,check when no record found in user list|`No results found` message is displayed|| ✅ ❌
1.35 |Check the `RESET FILTERS` button no fiters is applied on User list |`RESET FILTERS` button is disabled|| ✅ ❌
1.36 |Check the `RESET FILTERS` button when fiters is applied on User list |`RESET FILTERS` button is enabled|| ✅ ❌
1.37 |Click on search field,type `Device_$$`,check the `RESET FILTERS` button |`RESET FILTERS` button is enabled|| ✅ ❌
1.38 |Check the default pagination of User list |Default pagination is `25` records for User list|| ✅ ❌
1.39 |Click on the `Items per page` dropdown field |Dropdown opens|| ✅ ❌
1.40 |Check the other `Items per page` dropdown options|Dropdown options is `25`, `50`, `75`, `100`|| ✅ ❌
1.41 |Select `50` `Items per page` dropdown option|`50` records is displayed on User list|| ✅ ❌
1.42 |Check when any field name is too long|Name is displayed as tooltip|| ✅ ❌
1.43 |Check the User list sorting columns|User can sort list by using the following column names: `Full Name`,`Mobile#` & `Status`|| ✅ ❌
1.44 |Click on the `Full Name` sort icon|User list is sorted according to the selected column name|| ✅ ❌
1.45 |Click on the `Mobile #` sort icon|User list is sorted according to the selected column name|| ✅ ❌
1.46 |Click on the `Status` sort icon|User list is sorted according to the selected column name|| ✅ ❌

</details>

<details open>
   <summary><h2>2. User - Add  ✅ ❌ </h2></summary>

### Pre-condition
- This section is executed when user login in to the system.

## Actor 
- **Admin**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
2.01 |Click on the `ADD USER` button on User list screen |**Add user** dialog is opened|| ✅ ❌
2.03 |Check the dialog header|Screen header is **Add user**|| ✅ ❌
2.04 |Verify the details on **Add user** dialog|Dialog display following details: User details,Organization details,Accound configuration, `SAVE` & `CANCEL` button|| ✅ ❌
2.05 |Check all the mandatory fields on **Add user** dialog|All the mandatory fields are marked with (*)|| ✅ ❌
2.06 |Click on `Given name*` field |Field is clickable|| ✅ ❌
2.07 |Keep the `Given name*` field empty|User get an error message `Please enter at least 3 characters`|| ✅ ❌
2.08 |Enter a value between 3 to 50 characters : `A while backed I needed to count the amount letter` in `Given name*` field |Input value accepted|| ✅ ❌
2.09 |Enter `A while backed I needed to count the amount letters` in `Given name*` field|Last character `s` is truncate || ✅ ❌
2.10 |Click on `Family name` field |Field is clickable|| ✅ ❌
2.11 |Keep the `Family name` field empty|No error is displayed|| ✅ ❌
2.12 |Enter a value between 1 to 50 characters : `A while backed I needed to count the amount letter` in `Family name` field|Input value accepted|| ✅ ❌
2.13 |Enter `A while backed I needed to count the amount letters` in `Family name` field|Last character `s` is truncate || ✅ ❌
2.14 |Click on `Mobile number*` field |Field is clickable|| ✅ ❌
2.15 |Keep the `Mobile number*` field empty|User get an error message `Enter a valid mobile number`|| ✅ ❌
2.16 |Enter a value between 5 to 10 digits: `9936367755` in `Mobile number*` field|Input value accepted|| ✅ ❌
2.17 |Enter `99363677551` in `Mobile number*` field|Last digit `1` is truncate || ✅ ❌
2.18 |Enter a duplicate mobile number,Click on `SAVE` button when all mandatory fields are filled|User get an toast message `Duplicate mobile number`|| ✅ ❌
2.19 |Click on `Organization*` field|Dropdown options is displayed|| ✅ ❌
2.20 |Check the dropdown options|List is fetched from the backend|| ✅ ❌
2.21 |Keep the `Organization*` field empty|User get an error message `Please select a organization`|| ✅ ❌
2.22 |Select a organization from the dropdown options|Organization is selected|| ✅ ❌
2.23 |Select more than one dropdown options|Only one option at a time is selected|| ✅ ❌
2.24 |Click on `Role*` field|Dropdown options is displayed|| ✅ ❌
2.25 |Check the dropdown options|Dropdown options includes- `Front office staff`, `Device issuer`, `Healthcare provider`, `Admin` & `Analyst`|| ✅ ❌
2.26 |Keep the `Role*` field empty|User get an error message `Please select a role`|| ✅ ❌
2.27 |Select a role from the dropdown options|Role is selected|| ✅ ❌
2.28 |Select more than one dropdown options|Only one option at a time is selected|| ✅ ❌
2.29 |Check the default `Account configuration`|By default `Account configuration` is set to:**User account is active**|| ✅ ❌
2.30 |Click on the toggle button|`Account configuration` is set to:**User account is inactive**|| ✅ ❌
2.31 |Check the `SAVE` button when any mandatory field is not filled|`SAVE` button is disabled|| ✅ ❌
2.32 |Check the `SAVE` button when all mandatory field is filled|`SAVE` button is enabled|| ✅ ❌
2.33 |Click on the `CANCEL` button on **Add user** dialog screen|No new user is added,user navigates to the **User list**|| ✅ ❌
2.34 |Click outside of **Add user** dialog screen|**Add user** dialog is not closed|| ✅ ❌
2.35 |Fill all mandatory fileds,Click on the `SAVE`|A new user is created,user navigates to the **User list** with success toast message `User added successfully`|| ✅ ❌

</details>

<details open>
   <summary><h2>3. User - Edit  ✅ ❌ </h2></summary>

### Pre-condition
- This section can be executed when atleaset one user is registered to the system.To register a user execute TP (2.01 to 2.35).

## Actor 
- **Admin**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
3.01 |Click on the ✏️ edit button on User list screen |**Edit user** dialog is opened|| ✅ ❌
3.02 |Check the dialog header|Screen header is **Edit user**|| ✅ ❌
3.03 |Verify the details on **Edit user** dialog|Dialog display following details: Pre-filled data displayed during add/update,`SAVE` & `CANCEL` button|| ✅ ❌
3.04 |Check all the mandatory fields on **Edit user** dialog|All the mandatory fields are marked with (*)|| ✅ ❌
3.05 |Click on `Given name*` field |Field is clickable|| ✅ ❌
3.06 |Remove already entered `Given name*` & keep the field empty|User get an error message `Please enter at least 3 characters`|| ✅ ❌
3.07 |Enter a value between 3 to 50 characters : `A while backed I needed to count the amount letter` in `Given name*` field |Input value accepted|| ✅ ❌
3.08 |Enter `A while backed I needed to count the amount letters` in `Given name*` field|Last character `s` is truncate || ✅ ❌
3.09 |Click on `Family name` field |Field is clickable|| ✅ ❌
3.10 |Remove already entered `Family name` & keep the field empty|No error is displayed|| ✅ ❌
3.11 |Enter a value between 1 to 50 characters : `A while backed I needed to count the amount letter` in `Family name` field|Input value accepted|| ✅ ❌
3.12 |Enter `A while backed I needed to count the amount letters` in `Family name` field|Last character `s` is truncate || ✅ ❌
3.13 |Click on `Mobile number*` field |Field is clickable|| ✅ ❌
3.14 |Remove already entered `Mobile number*`& keep the field empty|User get an error message `Enter a valid mobile number`|| ✅ ❌
3.15 |Enter a value between 5 to 10 digits: `9936367755` in `Mobile number*` field|Input value accepted|| ✅ ❌
3.16 |Enter `99363677551` in `Mobile number*` field|Last digit `1` is truncate || ✅ ❌
3.17 |Enter a duplicate mobile number,Click on `SAVE` button when all mandatory fields are filled|User get an toast message `Duplicate mobile number`|| ✅ ❌
3.18 |Click on `Organization*` field|Dropdown options is displayed|| ✅ ❌
3.19 |Check the dropdown options|List is fetched from the backend|| ✅ ❌
3.20 |Update organization from the dropdown options|Organization is updated|| ✅ ❌
3.21 |Select more than one dropdown options|Only one option at a time is selected|| ✅ ❌
3.22 |Click on `Role*` field|Dropdown options is displayed|| ✅ ❌
3.23 |Check the dropdown options|Dropdown options includes- `Front office staff`, `Device issuer`, `Healthcare provider`, `Admin` & `Analyst`|| ✅ ❌
3.24 |Update role from the dropdown options|Role is updated|| ✅ ❌
3.25 |Select more than one dropdown options|Only one option at a time is selected|| ✅ ❌
3.26 |Check the last `Account configuration`|Last `Account configuration` is displyed|| ✅ ❌
3.27 |Click on the toggle button|`Account configuration` is changed|| ✅ ❌
3.28 |Check the `SAVE` button when any mandatory field is not filled|`SAVE` button is disabled|| ✅ ❌
3.29 |Check the `SAVE` button when all mandatory field is filled|`SAVE` button is enabled|| ✅ ❌
3.30 |Click on the `CANCEL` button on **Edit user** dialog screen|User details is not updated,user navigates to the **User list**|| ✅ ❌
3.31 |Click outside of **Edit user** dialog screen|**Edit user** dialog is not closed|| ✅ ❌
3.32 |Update & fill all mandatory fileds,Click on the `SAVE`|User details is updated,user navigates to the **User list** with success toast message `User details updated successfully`|| ✅ ❌
3.33 |Do not update the any user details,Click on the `SAVE`|User navigates to the **User list** with success toast message `User details updated successfully`|| ✅ ❌

</details>

</details>

<details open>
   <summary><h2>4. Disable User ✅ ❌ </h2></summary>

### Pre-condition
- This section can be executed when atleaset one user is registered to the system.To register a user execute TP (2.01 to 2.35).

## Actor 
- **Admin**

S No | Action                      | Expected Result | Actual Result (if different)  | Pass/ Fail
:-- | :--                          | :--             | :--                           | :--
4.01 |Click on `Active' toggle of a user in the **User list**|**Change status?** dialog is opened|| ✅ ❌
4.02 |Verify the details on **Change status?** dialog |User get text : `Are you sure you want to deactivate user account?` along with `NO, GO BACK` & `YES, CHANGE` button || ✅ ❌
4.03 |Click on `NO, GO BACK` button |Dialog is closed, user navgate to the **User list** screen|| ✅ ❌
4.04 |Click on `YES, CHANGE` button |User status changes to `Inactive`, dialog is closed, user navgate to the **User list** screen with success toast message `User status updated`|| ✅ ❌
4.05 |Check the status text after deactivating the user account in the **User list** |User status is `Inactive` on **User list** screen|| ✅ ❌
4.06 |Click on `Inactive' toggle  of a user in the **User list** |User status changes to `Active`,toast message displayed `User status updated`|| ✅ ❌
4.07 |Check the status text after activating the user account in the **User list** |User status is `Active` on **User list** screen|| ✅ ❌
