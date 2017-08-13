fullstack-nanodegree-vm
=============


Common code for the Relational Databases and Full Stack Fundamentals courses
----------------------------------------------------------------------------
#Installation Prerequisites:

1-download Git. 
2-download Virtual Box.
3-download Vagrant.
4-and install them.
#How to Run Vagrant on your PC:

1-Open Git bash terminal:
2-Move to your directory that the vagrantfile is located by entering cd vagrant/tournament.
3-Clone the virtual machine configurations
4-Run: git clone https://github.com/AliEid/Tournament

5-Start Vagrant by entering: vagrant up

#How to Run: 
.Once all steps above are complete, you can connect to the virtual machine.

1-Log into Vagrant virtual machine:
Run vagrant ssh
2-Move to tournament directory:
Enter cd /vagrant/tournament/
3-Create the required database:
Run psql -f tournament.sql
4-Launch Python command line:
Run python
5-Import tournament:
Run import tournament
6-to register a new player:
tournament.registerPlayer(player name)
7-to report a match results:
tournament.reportMatch(winner_id, loser_id)
8-to get pairings:
tournament.swissPairings()
9-to delete all players:
tournament.deletePlayers()
10-to delete all matches:
tournament.deleteMatches()
11-to get a list of the players and their win records:
tournament.playerStandings()
12-to test the project:
python tournament_test.py
this will create fake data to test the project, please re-create the database after test is completed
