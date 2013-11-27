#Scenarios where strong-naming is good
----------------------------
Add any scenarios where having/using strong-named open source assemblies is good
for you as a user, developer, or contributor.

Remember: We're only considering the case where strong-named assemblies have the full strong-name key
in the code repository.

If possible, keep scenarios on separate lines and put your username, name or email at the end of your scenario.
If you want to respond to a scenario, place your response right after the scenario and indent by one.

Example:

* Here is a scenario - username
  * A response to your suggestion - responder_username

--------------------------------
* Strong-named open source libraries can be used by other strong-named libraries and applications. - ericschultz
  * This is the scenario that drives most libraries to being strong-named. - robmen

* Rumor has it that GAC'd assemblies load faster and only strong-named libraries can be GAC'd. - robmen

* When the private key is protected strong-named open source libraries can define the "official release" vs. a "private build". - robmen
  * I know this does go against the note above but thought I'd get it captured. - robmen
    * Since strong-named assemblies are almost never validated in .Net 3.5, it's not that reliable an indictor. Also, making it easy for downstream users to try out (or use) modified assemblies in programs really fits the open source ethos better. I strongly recommend the use of code-signing to designate assemblies as official since it has no effect on binding. - ericschultz
