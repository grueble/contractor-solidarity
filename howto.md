# How to build and push dev changes:

1. hugo serve -D to run
2. do your development. remember to hard refresh localhost:1313 to see changes somewhat reliably
3. in config.toml, uncomment baseUrl for techcontracting and comment out the one for localhost:1313
4. add,commit, push changes in this repo for safekeeping
5. delete /public if it exists, then run just the bare "hugo" command to build a new /public
6. in deployment repo, take everything except the CNAME file and the .git folder and delete them.
7. drag everything from /public here into the deployment repo
8. add, commit, and push to master in deployment repo and you should be set to go.