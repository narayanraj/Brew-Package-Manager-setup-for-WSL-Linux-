# Brew-Package-Manager-setup-for-WSL-Linux
Brew Package manager setup a new profile in linux for managing software packages and their related dependencies smoothly.<p>
  
  Follow the Link to get complete help : <a href = "https://brew.sh/"> Brew-Home for Linux</a><br>
    
  After setting up Linux host/WSL, the best way to manage packages is Home-Brew profile.<br>
    <br>
    <b>Steps to be followed in Linux terminal :</b><br><br>
    1. Execute this command ( mentioned in above link )<br>
    command => <b> /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" </b>
    <br>This will install brew Package manager on linux system. It will create a new profile for installing packages.<br>
</br>
    2.  Run this set of commands in your terminal to add Homebrew to your PATH:<br>
    <b> <label>=> test -d ~/.linuxbrew && eval "$(~/.linuxbrew/bin/brew shellenv)" </br>
test -d /home/linuxbrew/.linuxbrew && eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)" </br>
test -r ~/.bash_profile && echo "eval \"\$($(brew --prefix)/bin/brew shellenv)\"" >>~/.bash_profile </br>
echo "eval \"\$($(brew --prefix)/bin/brew shellenv)\"" >>~/.profile </label></b> 
      <br><br>
      3. Browse for required Package - lets see nodejs<br>
      <b> command => brew search nodejs </b></br>
      This will provide with the packages available for nodejs from brew repo</br>
      </br>
      4. Choose the required from the list provided by above command and install :</br>
      <b>command =>  brew install node@14  </b></br>
      This will install nodejs in our example senario.</br>
      </br>
      5. To Reload bash's .profile without logging out run the below</br>
      <b> command => source ~/.profile</b></br>
      </br>
      6. Check for Node installation now in the system : </br>
      <b> command => node -v</b></br>
      This will display the nodejs version installed in this linux system under brew profile.
      <p><p>
  <b> Happy coding !!</b>
