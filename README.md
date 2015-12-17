# YGI Module
Powershell Module to enhance host display

## Write-Line
  A colored write-host
  * Display text in the host with a colored zone
  * Display text in the host with Colored border

### Examples
  * `Write-Line "The text between [bracket] is [Colored]"`
  * `Write-Line "This text will be displayed with border" -Border`
  * `Write-Line "The text between [bracket] is [Colored] but bracket are removed" -HideChar`
  * `Write-Line "The text between #sharp% and #percent% will be colored #sharp% and #percent% will not be displayed" -HideChar -OpenChar "#" -CloseChar "%"`
