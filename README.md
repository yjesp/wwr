<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Form </title>
    <link rel = "stylesheet" href="styles/style.css">

     
</head>
<body>
    <header>
       <a id="logo_link" href="index.html">
        <ima class="logo" src="images/logo.png" alt="Dry Oar Logo">
       </a>
       <nav>
           <a href="index.html">Home</a>
           <a href="rivers.html">Page 2</a>
           <a href="site-plan-rafting.html">Site Plan</a>
           <a href="contactus.html">Contact Us</a>
       </nav>
    </header>
    <div id="hero">
        <div id="hero-box">
            <img id="hero-img" src="images/hero.png" alt="People enjoying rafting">
        </div>
        <section id="hero-msg">
            <h1 class="home-title">Have An Adventure</h1>
            <h4>Make Memories with Dry Oar</h4>
            <div class='button-box'>
                <a class='book' href="contactus.html">Book Now</a>
            </div>
        </section>
    </div>
    <main>
      <div id="feedback"></div>
      <script>
        // get the feedback div element so we can do something with it.
        const feedbackElement = document.getElementById('feedback');
        // get the form so we can read what was entered in it.
        const formElement = document.forms[0];
        // add a 'listener' to wait for a submission of our form. When that happens run the code below.
        formElement.addEventListener('submit', function(e) {
            // stop the form from doing the default action.
            e.preventDefault();
            // set the contents of our feedback element to a message letting the user know the form was submitted successfully. Notice that we pull the name that was entered in the form to personalize the message!
            feedbackElement.innerHTML = 'Hello '+ formElement.user_name.value +'! Thank you for your message. We will get back with you as soon as possible!';
            // make the feedback element visible.
            feedbackElement.style.display = "block";
            // add a class to move everything down so our message doesn't cover it.
            document.body.classList.toggle('moveDown');
        });
      </script>
    
    </main>
<footer>
    <p>Dry Oar &copy; 20XX - Your First and Last Name Here</p>
    <p><a href="site-plan-rafting.html">Site Plan</a></p>
    <p><a href="contactus.html">Contact Us</a></p>
    <div class="social">
        <a href="https://facebook.com" target="_blank">
            <img src="images/facebook.png" alt="fb icon">
        </a>
        <a href="https://twitter.com">
            <img src="images/twitter.png" alt="twitter icon">
        </a>
        <a href="https://instagram.com">
            <img src="images/instagram.png" alt="instagram icon">
        </a>
    </div>
</footer>
</body>
</html>
