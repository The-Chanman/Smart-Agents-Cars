# Smart-Agents-Cars

# Software Setup
First things first the key thing you need to have is the particle-cli.
Best way of getting it is `npm install -g particle-cli`
If you don't have the npm command then you probably don't have node.js either. You should go download node.js at https://nodejs.org/en/
npm is included there. 

Once particle-cli is installed when you type particle in the terminal it should give you a lot of different commands. 
# Hardware Setup
Now the next part is you need to hookup the particle to your computer. 

1. Get the particle and attach the white usb-microusb cable from the computer to the particle board.
2. Take a small lithium ion battery (comes with the particle) and plug it into the particle board.
3. By now you should notice that the particle's central LED should be flashing different colors. It should start with White -> green -> cyan -> gently breathing cyan. If it flashes red that means your connection to 3G sucks, so either soldier through or go move it to a different area.
4. So now that your particle is connected we need to flash the new fireware to it. The one we are using is located in this git repo. First we need to put the electron into listening mode. So hold the *mode button for 3 second* on the electron. This should turn the central LED into a blinking dark blue light. If this worked skip to step 6.
5. If particle is being a little biatch and doesn't wanna go into listening mode. Hold *mode and the reset button down*. Now let go of the reset button. The central LED should turn purple and then yellow. Release the mode button when you see the central LED turn yellow. 
6. Now open up terminal. 
7. Navigate to where this git repo is on your computer using `cd` and `ls` commands for the inexperienced
8. Enter the command `particle flash --serial firmware.bin` then just follow the instructions that show up in the terimal. 
9. if it says flash success! Awesome. If it doesn't contact me at ecphylo@gmail.com