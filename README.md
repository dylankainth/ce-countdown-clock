# ce-countdown-clock
A BBC:Microbit based Countdown Clock

This project started in Summer 2019. The MicroBit ecosystem has changed a lot since then, so I can't guarantee that everything will still work the way it used to. 

## Set up

- A host MicroBit is programmed with the *'microbit-CE-Countdown-host'* file. 
  - This Microbit is confugired as the master microbit. It is in charge of timekeeeping and distributes radio signals to all the 'receiver' microbits. 
  - You must calibrate it with the amount of seconds until CE. That can be calculated using an [online calculator](https://www.timeanddate.com/date/timeduration.html).

- 9 Slave MicroBits are configured as receivers. Code for each one can be found in the *'receivers'* folder.
  - They simply receive signals from the host and display corresponding value on the screen.
  - The below table shows their radio configuration:

| Microbit Number | Microbit Radio | Showing Variable | Showing What? | Showing what? 2 |
| --------------- | -------------- | ---------------- | ------------- | --------------- |
| 1               | 247            | Day 3            | Day           | Hundreds        |
| 2               | 248            | Day 2            | Day           | Tens            |
| 3               | 249            | Day 1            | Day           | Units           |
| 4               | 250            | Hour 2           | Hour          | Tens            |
| 5               | 251            | Hour 1           | Hour          | Units           |
| 6               | 252            | Min 2            | Minutes       | Tens            |
| 7               | 253            | Min 1            | Minutes       | Units           |
| 8               | 254            | Sec 2            | Seconds       | Tens            |
| 9               | 255            | Sec 1            | Seconds       | Units           |
| 10              | Host           | Host             | Host          | Calculations    |

- I believe that the host microbit was mounted upside down for some reason?

## Make Changes!
You can edit the code by importing the files into the [MakeCode Editor](https://makecode.microbit.org/#editor)

If you're new to Github: Files can be downloaded by hitting the green Code button and then 'download zip'. Uncompress the file on your PC.

You can publish changes to this by making a github pull request to this repo. Learn more [here](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://www.youtube.com/watch%3Fv%3DtWkxc1eF36I&ved=2ahUKEwjdqbP7z5CGAxUkbEEAHTNCAvk4ChCjtAF6BAgDEAE&usg=AOvVaw2oZzQKLXJwgsGeJYeDMBzH)