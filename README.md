# Update-notification
Swift 3.2 &amp; up, IOS9 &amp; up, update notification for app which won't be published on the AppStore


# What you will need:
- A website which will contain the latest version of your app in plain text[(I Use 000webhost)](https://www.000webhost.com/)
  - [Example](https://dovydasberei.000webhostapp.com/public.html) 
- (Optional) A website which will cotain how to install your app 
  - [Example](https://dovydasberei.000webhostapp.com/how%20to%20install.html) 
- (Optional) A website which will cotain your ChangeLog in plain text
  - [Example](https://dovydasberei.000webhostapp.com/electricity%20run%20change%20log.html) 
- Swift 3.2 or later
- Xcode 
  
  
# How to install Update-notification:
1. Download *Check for update.swift*
2. Drag It to your Project
3. Use <kbd>cmd⌘</kbd> + <kbd>B</kbd> to build the project

# How to use Update-notification

``` Swift
        override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
        
        //basics:
        Update_Check.versionOfApp = 0.2
        
        Update_Check.webisite_containing_current_version = "https://dovydasberei.000webhostapp.com/public.html"
        
        check_for_update()
        
        
        // changable stuff:
        Update_Check.should_check_for_update = true
        
        Update_Check.show_changelog_as_an_option = true
        
        Update_Check.webisite_containing_changelog = "https://dovydasberei.000webhostapp.com/electricity%20run%20change%20log.html"
        
        Update_Check.show_how_2install_option = true
        
        Update_Check.webisite_containing_How2_install = "https://dovydasberei.000webhostapp.com/how%20to%20install.html"
        
        Update_Check.Use_diferent_View_controller = ViewController()
        
        Update_Check.update_messege = "New Version of Electricity Run came out,  please update to it when posible :)                                                                                                                                                                              CURENT VERSION: \(Update_Check.versionOfApp)                                                     -Admin"
        //     "\(versionOfApp)" displays versionOfApp
        
        Update_Check.update_title = ""
        // \(pm) displays webisite_containing_current_version number
        //change the update title on the 137 line of code, but i don't recomend to change it
        // How the title will apear: 1.1 Just came out
        
        Update_Check.change_log_popup_title = "Changelog"
    }
```

