# 🔗 Related issues
- ◀️ Prior step: [MY PATIENTS LIST VIEW](https://github.com/HimanshuKumarPal/SPC-Medical-Disability-Registry-main/blob/main/Usecases/MY%20PATIENTS%20LIST%20VIEW.md)  
- ▶️ Next step:  [MEDICAL HISTORY]() OR [FUNCTIONAL ASSESSMENT]()

# 📷 UI mockup
### [DISABILITY ASSESSMENT](https://www.figma.com/proto/uIJJwE09sapD6ERuuAoEVz/Vanuatu-MDR?type=design&node-id=58485-40060&t=ClC5melo1U8sbB0t-0&scaling=scale-down&page-id=53305%3A27555&starting-point-node-id=53837%3A32920)

# 📜 Workflow

Action | Result | Screen
-- | -- | --
Select a Patient from the list /Or After creating a new patient | User navigates to the **Patient landing** screen | ![image](https://github.com/HimanshuKumarPal/SPC-Medical-Disability-Registry-main/assets/90026796/aa51af3f-cde2-44d5-8386-62743b77cb2f)
Click on `Start assessment` button | User gets the **WG-SS disability** questions |![image](https://github.com/HimanshuKumarPal/SPC-Medical-Disability-Registry-main/assets/90026796/79ec41ff-e87d-4df2-baaa-ac6ca71b7ab9)
Click on the ❎ button | User navigates back to the **Patient landing** screen | ![image](https://github.com/HimanshuKumarPal/SPC-Medical-Disability-Registry-main/assets/90026796/aa51af3f-cde2-44d5-8386-62743b77cb2f)
Select any one option for a question | User can select any one option for a question |![image](https://github.com/HimanshuKumarPal/SPC-Medical-Disability-Registry-main/assets/90026796/6e3c70af-d9f9-4dce-8d9e-a9da150de033)
Do not answer any question | **`Save`** button is disabled | **NA**
Click on the **`Save`** button | User navigates **Patient landing** screen & gets the `Medical history` & `Functional assessment` cards|![image](https://github.com/HimanshuKumarPal/SPC-Medical-Disability-Registry-main/assets/90026796/49d8bd9a-b738-497e-a2f3-8783f6e09c41)


# ❗ Logic, Validation, and Messages
The [Washington Scale Short Survey](https://www.washingtongroup-disability.com/question-sets/wg-short-set-on-functioning-wg-ss/) asks the following six questions; all are mandatory:-

1. VISION: Do you have difficulty seeing, even if wearing glasses? 
2. HEARING: Do you have difficulty hearing, even if using a hearing aid(s)?
3. MOBILITY: Do you have difficulty walking or climbing steps?
4. COGNITION: Do you have difficulty remembering or concentrating? 
5. SELF-CARE: Do you have difficulty with self-care, such as washing all over or dressing? 
6. COMMUNICATION: Using your usual language, do you have difficulty communicating, for example understanding or being understood?

**Each question has one of four possible answers:**
- No difficulty
- Some difficulty
- A lot of difficulty
- Cannot do at all

##### NOTE - A newly created WG-SS record of a patient can be edited only on the same day. 
