# Contact US template (working)


Welcome to my sleek and efficient Contact Us page! I designed this template using a combination of HTML, CSS, JavaScript, and AJAX to provide users with a seamless and interactive way to reach out to us. What's more, we've incorporated the power of Google Drive, specifically Google Sheets, to effortlessly store and manage the incoming messages.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

 My sleek and efficient Contact Us page! I designed this template using a combination of HTML, CSS, JavaScript, and AJAX to provide users with a seamless and interactive way to reach out to us. What's more, we've incorporated the power of Google Drive, specifically Google Sheets, to effortlessly store and manage the incoming messages.

## Features

- User-Friendly Interface: My contact form is designed with a
    clean and user-friendly interface, making it easy for visitors to submit their inquiries or messages.


- Real-time Validation: JavaScript is employed for real-time
  form  validation, ensuring that users provide accurate and complete information before submission.


- AJAX for Smooth Interactions: The use of AJAX (Asynchronous
    JavaScript and XML) allows for a smooth and dynamic user experience. Messages are sent to the server without requiring a page refresh, providing instant feedback to users.

- Google Drive Integration: I've implemented a clever trick
  using Google Drive features. When users submit the contact form, their responses are automatically recorded in a Google Sheet and  also in your gmail inbox. This allows us to organize and manage incoming messages efficiently.


## Demo

You can access the live demo of the website at [here](https://vishnu1100.github.io/Contact-form/FIRST%20TRY%20ON%20THIS/).


## Technologies Used

- HTML
- CSS
- SCSS
- JavaScript
- Bootstrap
- Google Drive
- Ajax




## Font Styles

For this project, we used the following Google Fonts:

- [Montserrat](https://fonts.google.com/specimen/Montserrat) for headings and titles.
- [Roboto](https://fonts.google.com/specimen/Roboto) for the main content and descriptions.


## Installation

To run or install  this in your project locally,
  follow these steps carefully ( !! Carelessness leads to fatal error in app !!) :

1.  Open Google drive and create a new spread sheet 

![Screenshot 1](/screenshots/shot1.jpg)

2. Select the extensions menu and open app script

![Screenshot 2](/screenshots/shot2.jpg)

3. A new window will be opened like this 

![Screenshot 3](/screenshots/shot3.png)

4. Rename the existing code.gs file to script.gs 

![Screenshot 4](/screenshots/shot4.png)

![Screenshot 5](/screenshots/shot5.png)

5.  Blank out the existing code of script.gs and copy and paste the code from script.txt file from this repository , 


![Screenshot 6](/screenshots/shot6.png)

6. Change mail id according to your need 


![Screenshot 7](/screenshots/shot7.jpg)

7. Save the project 


![Screenshot 8](/screenshots/shot8.jpg)

8. Click deploy then new project

![Screenshot 9](/screenshots/shot9.png)

9. Just change  the description and deploy 

![Screenshot 10](/screenshots/shot10.png)

10. A popup will come just copy the webapp url from there dont lose it just copy and paste elsewhere (need it later :)


![Screenshot 11](/screenshots/shot11.jpg)

11. Thats all on the Googledrive now we can got to our project files

12.  Copy and paste this script code to your form index page  and add your early  copied code from drive  to the  url space,

!! please be carefully notice that your form id and the id in script are same,  in here  my id is #gform used in two places in script replace with yours !!

   ```bash
   <script>
      $("#gform").submit((e)=>{
          e.preventDefault()
          $.ajax({
              url:"yourcodehere",
              data:$("#gform").serialize(),
              method:"post",
              success:function (response){
                  alert("Form submitted successfully")
                  window.location.reload()
                  //window.location.href="https://google.com"
              },
              error:function (err){
                  alert("Something Error")
  
              }
          })
      })
  </script>
   ```
   

![Screenshot 12](/screenshots/shot12.jpg)

13. Dont forget to add this ajax library to head section 

   ```bash
   <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
   ```


![Screenshot 13](/screenshots/shot13.png)

14. YEAh its Done go and check out looser :) 




## Usage

   ```bash
   git clone https://github.com/vishnu1100/Vedhik_Healthcare.git
   ```

## Contributing

I  welcome contributions from the community to improve this website. If you find any bugs, have suggestions, or want to add new features, please follow these steps:

1. Fork this repository.

2. Create a new branch with a descriptive name:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Make your changes and commit them with clear commit messages.

4. Push your changes to your forked repository.

5. Create a pull request to the main repository, explaining the changes you made.

We appreciate your help in making this website better!




## Author

- Vishnu Santhosh  - [@vishnu](https://github.com/vishnu1100)




## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to modify this README file as per your requirements. Happy coding! If you have any questions or need further assistance, don't hesitate to reach out.
