# LunaBank – Web Application Testing

## About the project

This is a manual testing practice project based on the LunaBank web application.

For this project, I focused on the Login functionality and created test cases to check different login situations, including successful login, incorrect information, empty fields, account lock, invalid email format, and some edge cases.

The main purpose was to practice writing test cases, executing them, comparing the actual result with the expected result, and recording unexpected behavior.

## Testing scope

The test cases cover:

- Successful login with valid credentials
- Login with an incorrect password
- Empty required fields
- Partially empty login information
- Locked account
- Exceeding the allowed number of login attempts
- Invalid email format
- Editing previously entered login information

## Test cases

A total of **8 test cases** were created and executed.

| Result | Number |
|---|---:|
| PASS | 5 |
| FAIL | 3 |
| Total | 8 |

The test cases include:

- **Happy Path:** 1 case
- **Negative Cases:** 4 cases
- **Edge Cases:** 3 cases

## Test results

Most of the basic login scenarios worked as expected.

Three test cases were marked as **FAIL** because the actual behavior did not match the expected result:

- **TC_LOGIN_006 – Login thất bại khi nhập quá số lần giới hạn**  
  The system did not show a clear indication of the number of remaining attempts and did not temporarily lock the account as expected.

- **TC_LOGIN_007 – Login thất bại với Email sai định dạng**  
  An invalid email format resulted in the message `"Incorrect email or password."` instead of a message indicating that the email format was invalid.

- **TC_LOGIN_008 – Login với việc sửa lại dữ liệu nhập vào**  
  The login fields did not provide a convenient way to clear the entered information, and previously entered data had to be removed manually.

These results were recorded directly in the test case file together with the Actual Result, Status, Priority, and Notes.

## Test artifact

The complete test cases and execution results are available in the Excel file:

[**[Test Case LunaBank.xlsx](./Test%20Case%20LunaBank%286%29.xlsx)**](https://github.com/Thuwomai/LunaBank-Login-Test-Cases/blob/main/Test%20Case%20LunaBank.xlsx)

The Excel file contains:

- Test Case ID
- Test Case Name
- Module
- Precondition
- Test Steps
- Test Data
- Expected Result
- Actual Result
- Status
- Priority
- Notes

## What I practiced

Through this project, I practiced:

- Writing test cases from different user scenarios
- Creating positive, negative, and edge cases
- Preparing test data
- Executing test cases
- Comparing Expected Result and Actual Result
- Recording PASS/FAIL results
- Identifying unexpected application behavior
