🧾 Project: OrangeHRM Employee Details Automation (Selenium Java)
This project automates the process of adding and editing employee details on the OrangeHRM demo site using Selenium WebDriver in Java. It showcases handling various web elements such as text boxes, dropdowns, radio buttons, checkboxes, and buttons.

🎯 Key Features
1.Login to OrangeHRM using provided credentials
2.Navigate to the PIM module to add a new employee
3.Fill out registration details including login info
4.Edit personal details such as nationality, gender, marital status, and DOB
5.Handle form elements dynamically using Relative XPath locators
6.Demonstrate synchronization using waits
7.Support for multi-browser execution

🚀 How to Run This Project — Step by Step
🔧 1. Prerequisites
Before you begin, make sure you have the following installed:
✅ Java JDK (v8 or above)
✅ Eclipse IDE / IntelliJ IDEA / any Java IDE
✅ Maven (if using Maven) or Selenium JARs manually added
✅ Chrome Browser
✅ ChromeDriver (compatible with your browser version)

📦 2. Project Setup
* Clone or download the project from GitHub to your local machine
* Open the project in your preferred IDE

If you're using Maven, your pom.xml should include:

xml
<dependencies>
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>4.12.0</version>
    </dependency>
</dependencies>
If not, manually add Selenium .jar files to your project’s build path.

🌐 3. Configure WebDriver
Set system property for ChromeDriver:

java
System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");
💡 Tip: You can place chromedriver.exe in your project folder and reference it relative to your root directory.

📋 4. Login to the Application
Navigate to OrangeHRM Demo Site

Enter credentials:

Username: Admin

Password: admin123

Validate login success

🧑‍💼 5. Add Employee
Go to PIM > Add Employee

Enter First Name, Middle Name, Last Name

Slide Create Login Details

Fill in username and password

Click Save

📝 6. Edit Employee Details
Navigate to PIM > Employee List

Search and select the newly added employee

Click Edit

Update:

DOB

Gender (Radio Button)

Nationality (Dropdown)

Marital Status ("Single")

Click Save

📤 7. Logout and Close
Click on Profile Icon → Logout

Close the browser using driver.quit()

🧪 Optional Enhancements
✅ Add screenshot capture on success/failure

✅ Use WebDriverWait for robust synchronization

✅ Implement multi-browser support (Chrome, Firefox)

✅ Use Relative XPath to locate dynamic elements
