**Covert a tweet to speech and send it to an email or save it to
OneDrive**

**Prerequisites**

Azure subscription

Twitter account

Email account

Optional OneDrive

**Setting up**

Create a new logic App

All services -\> Integration -\> Logic Apps -\> Add

![](.//media/image1.png){width="6.294444444444444in"
height="3.154861111111111in"}

Chose the Subscription plan and the resource group (Click on Create new
if needed) then enter the desired Logic app name, chose the location
then click on Review + create -\> Create -\> Go to resource

![](.//media/image2.png){width="6.3in" height="3.0541666666666667in"}

From the side bar click on Logic App designer

![](.//media/image3.png){width="1.058824365704287in"
height="3.044750656167979in"}

In the search bar type Twitter then chose 'when a new Tweet is posted'

![](.//media/image4.png){width="2.7916535433070866in"
height="2.459892825896763in"}

Fill in the needed search (case sensitive for the Hashtag \# and name
tag @ ) then click on New step

![](.//media/image5.png){width="4.074866579177603in"
height="2.1763232720909884in"}

In the search bar type 'speech' then chose 'text to speech' (must have a
Speech cognitive service ready)

![](.//media/image6.png){width="3.8098906386701663in"
height="3.4278083989501313in"}

A new panel will open, chose the desired parameters for example

![](.//media/image7.png){width="5.064172134733158in"
height="2.3058070866141733in"}

Then click on New step and either choose type 'OneDrive' or 'Send to
Email'

For one drive chose one drive connecter and log in to your account.
Chose folder that you would like to add the generated audio files into
and type the file name, in the file content chose Audio file

![](.//media/image8.png){width="6.3in" height="2.6909722222222223in"}

For email option chose Send an email and login to your email address
then fill in the needed fields while adding the audio file as an
attachment

![](.//media/image9.png){width="4.279847987751531in"
height="3.5989304461942258in"}

Full scenario

![](.//media/image10.png){width="6.294444444444444in"
height="5.625694444444444in"}
