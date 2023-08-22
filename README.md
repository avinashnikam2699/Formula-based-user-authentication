# Formula-based-user-authentication
Nowadays as cyber security is a major concern for most of the web applications.So user authentication plays a very crucial role as security is concerned. In this project i have developed a "Formula/pattern based user authentication system" where during Registration/signing up user will be setting up his/her user id and formula instead of password.User would be creating a formula based on the variables who's values would be given in the form of a pin(formula pin) which will be generated by application server each time during user login. So by resolving the formula with the help of formula pin, user would be entering the formula value. So here every time user will be authenticating by entering a different formula value as application would be generating a different formula pin each time during user login. This code is just to simply demonstrate the idea of how an user authentication system can be made more safe,secured & effective by implementing formula based authentication instead of conventional password based authentication. Considering other security aspects as well this idea should be carefully implemented in actual applications, else other security loop-holes may be created.

User Signup :
During sign up process user would be entering his/her personal information with login credentials like username and would be generating a formula by following formula instructions which are mentioned in fig 1.1 below.User would be generating the formula based on 4 variables a,b,c & d and can also include some raw strings in between which the user needs to be placed outside the curly braces {} and operational/processing expressions inside the curly braces {}. Refer fig 1.1

User Login :
While login,user would be entering his/her username first. If the username is valid then application would generate a random 4 digit formula pin and evaluate the formula considering the 4 digit formula pin as variable values of a,b,c & d respectively. After calculating the formula value by application in the back end, application would display the 4 digit formula pin to the user and then user would be entering the formula value after resolving the formula with the help of formula pin.Then application would be matching the user calculated formula value and application calculated formula value.If this both values gets matched then application would allow the user to login successfully. Refer fig 1.2

fig 1.1
![image](https://github.com/avinashnikam2699/Formula-based-user-authentication/assets/142893800/60a1464b-b6df-46d1-b73c-a560f541aa9f)

fig 1.2
![image](https://github.com/avinashnikam2699/Formula-based-user-authentication/assets/142893800/5f599c40-f68c-4475-8d9c-84c93f2a791d)

# Some advantages of implementing this type of authentication idea :
1.Because of a user generated formula user would be entering each time a new formula value for respective formula pin received by user from application during login.This would make the authentication more secure.

2.Some cyber attacks which can be mitigated by this kind of authentication :

a) Social engineering attack like shoulder surfing : Even if an attacker gets to know the formula value of an user while login by shoulder surfing then too attacker won’t be able to derive or get to know the formula so easily with the help of formula value and formula pin if the user had generated a strong formula.

b) Keylogger attack : If an attacker has installed an keylogger software after user signup then while user login, attacker would be just able get the formula value by stealing user key strokes and not user formula.

c) Phishing attack : In phishing attack even if the attacker creates a fake application page and steals user formula value for the respective supplied formula pin by attacker, then further he would need to derive or get to know the user formula based on the formula pin and formula value which he has stealed. And this won’t be easy for an attacker to crack if user sets a strong formula.

3.User friendly : It will be easy for a user to remember a formula /pattern rather than a long string password.

4.This technique is simple to implement and effective from security perspective.

