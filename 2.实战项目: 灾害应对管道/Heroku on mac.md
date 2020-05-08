# Heroku on mac
## install Heroku on mac:
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % brew install heroku/brew/heroku 
Updating Homebrew...
==> Tapping heroku/brew
Cloning into '/usr/local/Homebrew/Library/Taps/heroku/homebrew-brew'...
remote: Enumerating objects: 129, done.
remote: Counting objects: 100% (129/129), done.
remote: Compressing objects: 100% (100/100), done.
remote: Total 1531 (delta 30), reused 128 (delta 29), pack-reused 1402
Receiving objects: 100% (1531/1531), 200.76 KiB | 45.00 KiB/s, done.
Resolving deltas: 100% (374/374), done.
Tapped 2 formulae (30 files, 269.6KB).
==> Installing heroku from heroku/brew
==> Installing dependencies for heroku/brew/heroku: heroku/brew/heroku-node
==> Installing heroku/brew/heroku dependency: heroku/brew/heroku
==> Downloading https://cli-assets.heroku.com/homebrew/node-12.16.2.t
#=#=#                                                                ##O#- #                                                              ##O=#  #                                                             #=#=-#  #                                                                                                                                                                                                      #                                                                    #                                                                    ###                                                                  ###                                                                  #####                                                                ######                                                               ########                                                             ##########                                                           ############                                                         ##############                                                       ###############                                                      ###############                                                      ##################                                                   #####################                                                #####################                                                #######################                                              ########################                                             #########################                                            ############################                                         ############################                                         #############################                                        ##############################                                       #################################                                    ##################################                                   #####################################                                #####################################                                #######################################                              #########################################                            ##########################################                           ############################################                         ###############################################                      ###############################################                      ################################################                     ###################################################                  ####################################################                 #######################################################              #######################################################              #######################################################              ##########################################################           ###########################################################          ##############################################################       ##############################################################       #################################################################    ##################################################################   ################################################################################################################################################################################################################################################################################################################################################################################################################################# 100.0%
🍺  /usr/local/Cellar/heroku-node/12.16.2: 3 files, 42.2MB, built in 22 seconds
==> Installing heroku/brew/heroku
==> Downloading https://cli-assets.heroku.com/heroku-v7.40.0/heroku-v
#=#=#                                                                ##O#- #                                                              ##O=#  #                                                                                                                                                                                                       #                                                                    #                                                                    ###                                                                  #####                                                                ######                                                               #######                                                              #######                                                              #########                                                            #########                                                            ###########                                                          ############                                                         ############                                                         #############                                                        ###############                                                      ###############                                                      ###############                                                      ##################                                                   ##################                                                   #####################                                                #######################                                              #########################                                            ##########################                                           ###########################                                          ############################                                         #############################                                        ##############################                                       ###############################                                      #################################                                    ##################################                                   ####################################                                 ######################################                               #######################################                              ########################################                             ##########################################                           ###########################################                          ############################################                         ###############################################                      #################################################                    ###################################################                  ####################################################                 #####################################################                ######################################################               #######################################################              #########################################################            ############################################################         #############################################################        #################################################################    #################################################################    ####################################################################################################################################################################################################################################################################################### 100.0%
==> Caveats
To use the Heroku CLI's autocomplete --
  Via homebrew's shell completion:
    1) Follow homebrew's install instructions https://docs.brew.sh/Shell-Completion
        NOTE: For zsh, as the instructions mention, be sure compinit is autoloaded
              and called, either explicitly or via a framework like oh-my-zsh.
    2) Then run
      $ heroku autocomplete --refresh-cache

  OR

  Use our standalone setup:
    1) Run and follow the install steps:
      $ heroku autocomplete

Bash completion has been installed to:
  /usr/local/etc/bash_completion.d

zsh completions have been installed to:
  /usr/local/share/zsh/site-functions
==> Summary
🍺  /usr/local/Cellar/heroku/7.40.0: 18,739 files, 46.5MB, built in 1 minute 35 seconds
==> Caveats
==> heroku
To use the Heroku CLI's autocomplete --
  Via homebrew's shell completion:
    1) Follow homebrew's install instructions https://docs.brew.sh/Shell-Completion
        NOTE: For zsh, as the instructions mention, be sure compinit is autoloaded
              and called, either explicitly or via a framework like oh-my-zsh.
    2) Then run
      $ heroku autocomplete --refresh-cache

  OR

  Use our standalone setup:
    1) Run and follow the install steps:
      $ heroku autocomplete

Bash completion has been installed to:
  /usr/local/etc/bash_completion.d

zsh completions have been installed to:
  /usr/local/share/zsh/site-functions
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % heroku login 
heroku: Press any key to open up the browser to login or q to exit: 
Opening browser to https://cli-auth.heroku.com/auth/cli/browser/e6678bbb-0a2d-449f-a739-2913ac1dd626
Logging in... done
Logged in as 1564468177glen@gmail.com
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % 
```
Getting Started on Heroku with Python SEt up
<br>https://devcenter.heroku.com/articles/getting-started-with-python#set-up
