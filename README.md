# medical-appointment
The dataset medical_appointment_no_shows.xlsx contains information about patients medical appointments, including whether or not the patient showed up for their appointment. The purpose of cleaning this dataset is to ensure data accuracy, consistency, and readiness for analysis.

## Data Cleaning Objectives

The data cleaning process aimed to:

* Eliminate errors and inconsistencies
* Format and standardize data
* Handle missing, duplicate, or invalid entries
* Prepare the dataset for further statistical or visual analysis

---

## Cleaning Steps Performed in Excel

### 1. Removed Duplicates

* Used Excel’s "Remove Duplicates" feature to eliminate repeated entries based on key columns: `PatientId`, `AppointmentID`, and `ScheduledDay`.

### 2. Corrected Column Names

* Renamed headers for clarity and consistency:

  * `No-show` was changed to `No_Show`
  * Removed extra spaces from all column names

### 3. Formatted Date Columns

* Converted `ScheduledDay` and `AppointmentDay` from text to proper date format using Excel’s `DATEVALUE()` and formatting tools.
* Created a new column `Waiting_Days` to calculate the number of days between the scheduled date and the appointment date.

### 4. Checked for Null or Missing Data

* Used filtering and `ISBLANK()` function to locate missing values.
* Assessed if missing values should be removed or addressed with imputation based on column importance.

### 5. Cleaned Categorical Variables

* Ensured consistency in `Gender` values (e.g., all entries are either `M` or `F`)
* Standardized neighborhood names for uniform spelling and formatting

### 6. Created New Analytical Columns

* Added the following derived fields:

  * `Waiting_Days` (difference between scheduled and appointment dates)
  * `Weekday` (day of the week of the appointment)
  * `Age_Group` (categorized age into defined groups: 0–18, 19–35, etc.)



