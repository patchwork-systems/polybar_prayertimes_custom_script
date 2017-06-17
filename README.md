# Check Athan for Polybar

Check Athan for Polybar is a simple custom script for getting the current and
next Islamic prayer times and displaying them in
[Polybar](https://github.com/jaagr/polybar).

The script works using urllib to request a JSON object of all prayer times,
iterating through the JSON object checking if for the next and current times,
converting the times into 12 hour format, then finally displaying the times. 

The polybar configuration for this script can be as shown below:

```
[module/athan]                                                                  
type = custom/script                                                            
exec = ~/.config/polybar/scripts/check-athan/check-athan         
interval = 60  

```
