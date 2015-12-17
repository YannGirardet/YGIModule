# YGI Host Module
Powershell Module to enhance host display
* Write-Line
* Write-ChoiceMenu
  * Add-ChoiceItem
* Ask-User

## Write-Line
  A colored write-host
  * Display text in the host with a colored zone
  * Display text in the host with colored border

### Examples
  * `Write-Line "The text between [bracket] is [Colored]"`
  * `Write-Line "This text will be displayed with border" -Border`
  * `Write-Line "The text between [bracket] is [Colored] but bracket are removed" -HideChar`
  * `Write-Line "The text between #sharp% and #percent% will be colored #sharp% and #percent% will not be displayed" -HideChar -OpenChar "#" -CloseChar "%"`

## Add-ChoiceItem
  Create ChoiceItem to use with Write-ChoiceMenu
  * Create a Menu item that return a string

### Examples
  * `$ChoiceMenu = Add-ChoiceItem -MenuItem "Get the process list" -MenuAction "Get-Process"`
  * `$ChoiceMenu = Add-Choice -Menu $ChoiceMenu -MenuItem "Get the time" -MenuAction "Get-Date -Format HH:mm:ss"`
  * `$ChoiceMenu = Add-Choice -Menu $ChoiceMenu -MenuItem "Get the date" -MenuAction "Get-Date -Format dd.MM.yyyy"`

## Write-ChoiceMenu
  A Choice Menu creator
  * Create a Menu into host where user have to select between different choice defined by Add-ChoiceMenu
    * Return $null if user choose to exit

### Example
  * `$ReturnValue = Write-ChoiceMenu -Menu $ChoiceMenu`

## Ask-User
