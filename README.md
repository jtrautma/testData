# testData
Contains or generates data for the purpose of software testing

Address Data
=====================================================

# Motivation
Because of continously improving ident processes, you may need to diversify address data between test runs or let your test customers reside in different places. How many different post codes do you know off the top of your head? Exactly -- that's where this random zip code generator comes in handy.

# Purpose
The **/AddressData** sub-project contains a list of all valid post codes for the country specified. Run this program everytime you need an address and you will be given a ZIP code or PLZ, a city name (useful if post code is shared by several cities to use autofill), as well as a randomly selected street name (Germany only). Afterwards the _used up_ post code will be added to a list of zip codes already displayed to you in previous runs of the program. For future runs, these codes will be skipped.

# Run the program [GERMANY]
Please execute the "**START.ps1**" file in *Powershell*. It will randomly select a PLZ from the 8,000+ ones there are in Germany. If, by any chance, the selected PLZ has been picked for you in a previous run of this program, that "used" PLZ and city pair will be printed, however, the program continues until a "fresh" PLZ is found. <br />
Powershell comes with every Windows machine; for installing it on a Mac, please refer to https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell-core-on-macos?view=powershell-6. <br />
If Powershell refuses to run scripts, you will need to relax the script execution policy (see https://github.com/jtrautma/powershell/blob/master/README.md for the necessary steps).

# Reset [GERMANY]
In case all available PLZs have been consumed by you (which is highly unlikely to happen), the program will inform you about it. To clear the list of PLZs already seen, please feel free to run the "reset_plz.ps1" script in the "reset" folder.

# Escape
If you wish to quit the program execution prematurely, use **CTRL** + **C**
