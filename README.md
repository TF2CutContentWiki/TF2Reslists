# TF2Reslists
Update history of tf/reslists contents from September '07 build until the May 13, 2013 patch when the directory and its contents were finally removed from the game.

# Statistics
* In total, for chunk 441 (team fortress 2 content) there are 396 manifests (patches) to go through.
  * I've stopped at 197 (Australian Christmas) for today, will continue from there tomorrow.

# Interesting Recent Finds
* [All the commits in general](https://github.com/404UNFca/TF2Reslists/commits/master).
  * I've left a comment on each commit explaining when I think each manifest (patch) is from.
* Most recently, the [Australian Christmas Update diff](https://github.com/404UNFca/TF2Reslists/commit/148e3428845c22c1eca4b03deac54b6c5b14523a)
  * Load the diffs for reslists/cp_degrootkeep.lst, and reslists/cp_degrootkeep.snd. You can CTRL+F for my username to find comments I've left throughout both files in the diff explaining what is of interest.

# FAQ
Q: Where do you get these old files?

A: From [this spreadsheet](https://docs.google.com/spreadsheets/d/1nrf9eDrGGKlB16_8RR-Fq1ERu5PinhDa-HQnFAqVSZM/edit#gid=1648607917). Specifically, you're gonna want to check the TF2 Pre-Steampipe tab at the bottom. Thanks to a very great individual and a collector of builds of a ton of Source Engine games, Firebeast, we have a collection of every TF2 build from release up until Steampipe was introduced in 2013.

However, it's stored in chunk & manifest form, similarly to how downloads are issued over Steam. Because of this, it's quite hard to figure out which patch date a manifest corresponds to. You can't just take the manifest # and correspond that to "it's the #th patch". Chunk 442 and 443 for example are the "team fortress 2 materials" and "team fortress 2 client content" packages. Chunk 442 has 227 manifests, and chunk 443 has 342. Note the inequality in the # of manifests between the three chunks. Trying to rebuild full patches from these 3 separate chunks would be impossible. The best option you have for locating content from a specific patch is using the extraction Python script to try to narrow down which manifest is a specific patch based on "does this file which was added on this patch appear in this manifest or not?", since you can specify a certain directory or file to extract instead of the entirety of the manifest.
