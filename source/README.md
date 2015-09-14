



This was initially a four person group project. After collaborating on different ideas, we agreed that two of the members would work on other projects. If at any point myself and the other member need help or input, we would come together as a complete group to get it resolved. 

The idea was to create a basic survey app. Features would be added in the form as different types of survey questions. The most difficult feature was creating the multiple choice question. We wanted to give the user the option to easily add and subtract the number forms the could use by clicking + or -. This was the only time we came together as a complete group.

The rest of the app was fairly straight forward. The only thing I didn't work on was implementing bootstrap. One of the members came in at the end to work on the CSS while I finished up the code for the voting feature.

HOW TO RUN

You can go to http://surveygopher.herokuapp.com/

or

To run this on your local server you should have shotgun installed:

1. $ install shotgun

2. Navigate to the survey_gopher/source file in the terminal:
	* $ bundle install
	* $ be rake db:create
	* $ be rake db:migrate

3. Start the shotgun server:
	* $ be shotgun

4. In your browser type: http://localhost:9393/

Note:
You must register a username and password. There is no acknowledgement as long as it's successful.
Then you can use it to log in. There are no validations so use whatever you want.

Problems running server?

If shotgun is already running kill it by first:
 * $ ps ax | grep shotgun
 * $ kill -9 XXXX
 	- XXXX should be replaced with the digits preceding the filepath

 If postgres server is not running you can copy the line below and enter it in your terminal
 	
 	pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start
