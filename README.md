# OpenSimCurrencyServerNet

This implementation removes the ability to use the BUY MONEY button in viewers.

This is a custom build from https://github.com/ManfredAabye/opensimcurrencyserver-dotnet for the Canadian Grid

Will work on improving this repo as I go.

### All components have been tested for stability as far as possible with my server.

### Buying land without landtool.php is now possible.

### Buying currency without currency.php is now possible.

## OpenSim Currency Server for OpenSim 0.9.3.1 Dev
Windows Linux IOS DotNet 6.0 & Windows Linux IOS DotNet 8.0

(Ubuntu 18 = DOTNET 6.0 - Ubuntu 20+ DOTNET 8.0)

Everything works so far.

The MoneyServer intercepts the helper messages and processes them internally.

     ; helper uri (for currency.php and landtool.php):
     economy = ${Const|BaseURL}:8008/
     
Testing Firestorm Viewer for OpenSim 7.1.11.76496 works.

### From the original DTL/NSL Money Server
by Fumi.Iseki and NSL http://www.nsl.tuis.ac.jp , here is a test revision for DotNet6 & DotNet8.

## New:

     ; General maximum:
     CurrencyMaximum = 20000;
     ; Turn on money purchase = on turn off = off.
     CurrencyOnOff = on;
     
     ; Buy money only for group true/false:
     CurrencyGroupOnly = true;
     ; Buy money only for group the group ID
     CurrencyGroupID = "00000000-0000-0000-0000-000000000000";
     
     ; Verify the email address and anyone without it cannot buy money.
     UserMailLock = true;

## TODO:
Various functions are still missing.

     ; Maximum per day:
     TotalDay = 100;
     ; Maximum per week:
     TotalWeek = 250;
     ; Maximum per month:
     TotalMonth = 500;
