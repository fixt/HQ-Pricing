To run the HQ-Pricing. Simply make sure that you have all the required imports. For a list, please review requirements.txt. 

Click on Kernel and then Restart & Run All.

If an error occurs, most likely it because one of the pricing websites have changed their description. You will need to update the 
offending description and then rerun the script.

Additional notes:

# iPhoneX
iPhoneX = HQPricing('iPhone X', 'Battery', 
df_defender[df_defender['Description'] == 'Battery for iPhone X']['Price'].iloc[0:1].tolist()[0],
df_gadgets[df_gadgets['Description'] == 'Battery for the iPhone X']['Price'].iloc[0:1].tolist()[0], 
df_sentrix[df_sentrix['Description'] == 'Replacement Battery For iPhone X (Premium Quality, AmpSentrix)']['Price'].iloc[0:1].tolist()[0])

The update a description simply replace it for the given website. For example, if one wants to change the 'Battery for iPhone X'
description for www.defender.com, simply change it to the correct text and rerun.

If you need to add a new device, simply following the structure above for the iPhone X. Then add the device to the following list:

phones = [iPhoneX, iPhone8, iPhone7, iPhone6, iPhone5, iPhone5C, iPhone5S, iPhone6S, iPhoneSE, 
          iPhone7Plus, iPhone6Plus, iPhone6SPlus, iPhone8Plus, iPhone5_Screen, iPhone5C_Screen,
          iPhone5S_Screen, iPhone6_Screen, iPhone6Plus_Screen, iPhone6S_Screen, iPhone6SPlus_Screen, 
          iPhone7_Screen, iPhone8_Screen, iPhone7Plus_Screen, iPhone8Plus_Screen, iPhoneSE_Screen,
          iPhoneX_Screen, iPhone7Plus_charging, iPhone7_charging, iPhone8_charging, iPhone8Plus_charging,
          iPhone6SPlus_charging, iPhone6S_charging, iPhoneX_charging, iPhoneSE_charging, iPhone5_charging,
          iPhone5C_charging, iPhone5S_charging, iPhone6_charging, iPhone6Plus_charging, iPhone5_Home,
          iPhone5C_Home, iPhone5S_Home, iPhoneSE_Home, iPhone6S_Home, iPhone6SPlus_Home, iPhone6Plus_Home,
          iPhone6_Home, iPhone7_Home, iPhone7Plus_Home, iPhone8Plus_Home, iPhone8_Home,
          iPadAir2_Screen, iPadAir2_Battery, iPadAir2_Home, iPadAir2_charging, iPad5_Home, iPad5_charging,
          iPad5_Screen, iPad6_Screen, iPad6_charging, iPad6_Home, iPad5_Battery, iPad6_Battery,
          iPad5_Digitizer, iPad6_Digitizer, iPad5_Display, iPad6_Display, iPhoneXR_Screen, iPhoneXR_charging,
          iPhoneXS_Screen, iPhoneXS_charging, SamsungNote9_Screen, SamsungNote9_Battery, SamsungNote9_charging,
          SamsungGS9_Screen, SamsungGS9_Battery]
          
If you have further questions, please contact me.

