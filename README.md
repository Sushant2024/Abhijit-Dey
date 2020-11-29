# Portfolio-themes
Various Themes for Portfolio

Website: [preview](https://sushant2024.github.io/CV/)

**Live share**: [joining_link](https://prod.liveshare.vsengsaas.visualstudio.com/join?9DB09C293AB31D79A65E877916AEB2B8690A)

Resource: [Resource](https://sites.google.com/view/sumit-bhowmik/home?authuser=0)
# Latest Release:
- **beta version** : [version1.0.1](https://github.com/Sushant2024/portfolio-themes/releases)

# Published Packages:
- None yet

# Resource:

## Mailing System:
- **[Tutorial](https://www.youtube.com/watch?v=w4-EWgo-nhw)**
- [Formspree](https://formspree.io) - Mails content to your mail (available in spam of your mail-account by default)
- [Formcarry](https://formcarry.com/) - Mails content to your mail-ID
- [EmailJS](https://www.emailjs.com/) - Mails content to location you want (gmail, icloud, outlook, yahoo, etc)

## Making Contents:
- [Book effect](https://youtu.be/pvbC5kLp7OQ)
- [Timeline effect](https://youtu.be/9IhZiupGNiA)
- [Service Section](https://youtu.be/twvWRXbj_qI)

## Code for countdown timer :

- HTML code to be entered in header under body

    `<h3 style="text-align: center; color: aqua;">UNDER MAINTENANCE!</h3>`<br>
    `<h3 id="demo" style="text-align: center; font-size:larger; color: cyan;"></h3>`

- JAVASCRIPT CODE for countdown

         <script>
            // Set timer we are counting down to [date month year or time]
            var countDownDate = new Date("Nov 30, 2020 00:00:00").getTime();

            // Update the count down every second
            var countDownfunction = setInterval(function(){

                // get Today's date and time
                var now = new Date().getTime();

                // Find distance between now and the countdownDate
                var distance = countDownDate - now;

                // Time calculations for days, hours, minutes and seconds
                var days = Math.floor(distance / (1000 * 60 * 60 * 24));
                var hours = Math.floor((distance % (1000 * 60 * 60 * 24))/ (1000 * 60 * 60));
                var minutes = Math.floor((distance % (1000 * 60 * 60))/ (1000 * 60));
                var seconds = Math.floor((distance % (1000 * 60)) /1000);

                // Result will be displayed in "div" with "id=demo"
                // Output the result in an element with id="demo"
                document.getElementById("demo").innerHTML = days + "d " + hours + "h " + minutes + "m " + seconds + "s ";

                // If the count down is over, write some text
                if(distance < 0) {
                clearInterval(countDownfunction);
                document.getElementById("demo").innerHTML ="EXPIRED!";
                }
            }, 1000)
        </script>