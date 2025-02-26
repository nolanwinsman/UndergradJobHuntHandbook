# Miscellaneous Advice

---

This is mostly just advice I would give to people that just landed a position.

- Get your finances figured out. Most people have poor money management skills. Don't be like them. Live below your means to some degree.
- Learn how to invest your money. This is one of those things that will be the smartest choice you ever make and old you will be quite happy. I can't tell you what to invest in (you should open a ROTH IRA though) Just watch a lot of Youtube videos on it and dedicate some amount of money every month to go into investments.
- Reach out to a lot of people for advice. Reaching out to me is smart since I know what I'm talking about. I still reach out to a lot of family, friends, and former bosses for advice.
- Learn to cook for yourself. You might land a large tech salary. Don't be one of the people that spends a quarter of it on UberEats.
- The terminal is your friend. I know a lot of people avoid the terminal as much as possible when programming, but the more you use it, the more you realize how incredible it is. Get used to doing things in the terminal
- [Neovim](https://neovim.io/) is incredible. A majority of people will not enjoy writing their code in Neovim, but I love it. If you're willing to put in the time, you can become a lot faster at writing code.
- Focus on automating as much as possible. As you get older more and more responsibility will be thrown your way. With your computer skills, you should be able to automate a lot of it. Start simple by automating payments/bills and work your way up to automating as much as possible.

## Learning the Wrong Lessons

## The Terminal is Your Friend

I remember the first time I tried to use a computer terminal. It was back in my teenage years. I was trying to setup a raspberry pi to play retro games on. The terminal was quite daunting and spooky to me. Years later, I do as much as I can in my computer terminal
since it's so much faster and more automatable. Some could say my computer terminal is my best friend. Also you look sick as heck working in the terminal so that's important too.

Here's a simple example. Let's say you just booted a brand new computer and you want to install Google Chrome. Normally you would open your current browser, then search **Google Download** find the right page then download the file. Lastly you would run the executable.
Now this works fine, but what if you're a school that got 100 new computers and each of those computers needed 100 different pieces of software installed. It could take dozens of hours to get all the computers setup.

Now here's how you would install Google Chrome through a Linux terminal. The process is similar with Winget for Windows and Brew for Mac.

```sh
sudo apt install google-chrome-stable
```

That's it, one little command in the terminal to install Google Chrome. Now for installing 100 pieces of software, you could write a simple script like below

```sh
#!/bin/bash

# List of software packages to install (only five packages in this example)
packages=(
    "google-chrome-stable"
    "vlc"
    "git"
    "curl"
    "nvim"
)

# Update package list
sudo apt update

# Install each package in the list
for package in "${packages[@]}"; do
    echo "Installing $package..."
    sudo apt install -y "$package"
done
```

Now in an enterprise scenario they use something a bit more advanced than this, but it's not too far off. This is just one of a trillion examples of why using the terminal is advantagious to you.

## General Computer Competency is Underrated

One thing that not I feel a lot of CS majors don't think about is the value of being good with computers. I've seen a lot of people waste a lot of time not knowing how to do something simple. Being competent with computers can also make you work a lot faster. I can't
imagine a world where I didn't know the shortcuts I know.

Here is a small checklist of things that if you answer "No" to all of them you might want to spend more time on computers.

- Can you change an environmental variable on your computer and do you know what that means?
- Do you know how to recover a tab you accidentally closed on your browser with one input?
- Can you install an operating system on a computer?
- Can you SSH into a computer?
- When you go to install new software, do you first look at the Microsoft store? (The answer to this should be "No")
- Do you know how to SCP some files from one computer to another?
- Do you know what a VPN is and does?

These are far from perfect questions but hopefully you get my point.

## Swiss Cheese Knowledge

## Luck
