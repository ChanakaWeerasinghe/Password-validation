# Password-validation
javascript password validation 



      checkPassword(pw) {
        console.log(pw);
              // Validate lowercase letters
         var lowerCaseLetters = /[a-z]/g;
          // Validate capital letters
          var upperCaseLetters = /\w*[A-Z]\w*[A-Z]\w*/g;
      // Validate numbers
        var numbers = /[0-9]/g;
         //valiodate special caracters
         var special = /\W|_/g;
        if (pw.match(special) && pw.match(lowerCaseLetters) && pw.length >= 8 && pw.match(upperCaseLetters) && pw.match(numbers)) {
        console.log("validated");
        this.isvalidpw=true;
        
      } else {
        this.isvalidpw=false;
        console.log("not validated");
      }
     }
