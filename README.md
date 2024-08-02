# AI
We have extensive experience in the field of cryptocurrencies, forex trading 
2024-06-27T06:37:02.0520063Z Current runner version: '2.317.0'
2024-06-27T06:37:02.0545383Z ##[group]Operating System
2024-06-27T06:37:02.0546162Z Ubuntu
2024-06-27T06:37:02.0546505Z 22.04.4
2024-06-27T06:37:02.0546810Z LTS
2024-06-27T06:37:02.0547229Z ##[endgroup]
2024-06-27T06:37:02.0547609Z ##[group]Runner Image
2024-06-27T06:37:02.0548014Z Image: ubuntu-22.04
2024-06-27T06:37:02.0548479Z Version: 20240616.1.0
2024-06-27T06:37:02.0549509Z Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20240616.1/images/ubuntu/Ubuntu2204-Readme.md
2024-06-27T06:37:02.0550902Z Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20240616.1
2024-06-27T06:37:02.0551843Z ##[endgroup]
2024-06-27T06:37:02.0552261Z ##[group]Runner Image Provisioner
2024-06-27T06:37:02.0552813Z 2.0.370.1
2024-06-27T06:37:02.0553122Z ##[endgroup]
2024-06-27T06:37:02.0555390Z ##[group]GITHUB_TOKEN Permissions
2024-06-27T06:37:02.0557072Z Actions: write
2024-06-27T06:37:02.0557681Z Attestations: write
2024-06-27T06:37:02.0558256Z Checks: write
2024-06-27T06:37:02.0558652Z Contents: write
2024-06-27T06:37:02.0559107Z Deployments: write
2024-06-27T06:37:02.0559474Z Discussions: write
2024-06-27T06:37:02.0559868Z Issues: write
2024-06-27T06:37:02.0560284Z Metadata: read
2024-06-27T06:37:02.0560649Z Packages: write
2024-06-27T06:37:02.0561016Z Pages: write
2024-06-27T06:37:02.0561441Z PullRequests: write
2024-06-27T06:37:02.0561838Z RepositoryProjects: write
2024-06-27T06:37:02.0562282Z SecurityEvents: write
2024-06-27T06:37:02.0562768Z Statuses: write
2024-06-27T06:37:02.0563130Z ##[endgroup]
2024-06-27T06:37:02.0566378Z Secret source: Actions
2024-06-27T06:37:02.0567066Z Prepare workflow directory
2024-06-27T06:37:02.1291917Z Prepare all required actions
2024-06-27T06:37:02.1448607Z Getting action download info
2024-06-27T06:37:02.3960695Z Download action repository 'actions/checkout@v3' (SHA:f43a0e5ff2bd294095638e18286ca9a3d1956744)
2024-06-27T06:37:02.5327622Z Download action repository 'actions/setup-go@v4' (SHA:93397bea11091df50f3d7e59dc26a7711a8bcfbe)
2024-06-27T06:37:03.1702506Z Complete job name: check-codebase
2024-06-27T06:37:03.2637695Z ##[group]Run actions/checkout@v3
2024-06-27T06:37:03.2638438Z with:
2024-06-27T06:37:03.2638844Z   repository: jesseduffield/lazygit
2024-06-27T06:37:03.2639713Z   token: ***
2024-06-27T06:37:03.2640094Z   ssh-strict: true
2024-06-27T06:37:03.2640532Z   persist-credentials: true
2024-06-27T06:37:03.2641108Z   clean: true
2024-06-27T06:37:03.2641508Z   sparse-checkout-cone-mode: true
2024-06-27T06:37:03.2642050Z   fetch-depth: 1
2024-06-27T06:37:03.2642530Z   fetch-tags: false
2024-06-27T06:37:03.2642907Z   lfs: false
2024-06-27T06:37:03.2643307Z   submodules: false
2024-06-27T06:37:03.2643809Z   set-safe-directory: true
2024-06-27T06:37:03.2644251Z env:
2024-06-27T06:37:03.2644617Z   GO_VERSION: 1.22
2024-06-27T06:37:03.2644987Z   GOFLAGS: -mod=vendor
2024-06-27T06:37:03.2645488Z   GOARCH: amd64
2024-06-27T06:37:03.2645889Z ##[endgroup]
2024-06-27T06:37:03.5197172Z Syncing repository: jesseduffield/lazygit
2024-06-27T06:37:03.5199115Z ##[group]Getting Git version info
2024-06-27T06:37:03.5200007Z Working directory is '/home/runner/work/lazygit/lazygit'
2024-06-27T06:37:03.5200818Z [command]/usr/bin/git version
2024-06-27T06:37:03.5258218Z git version 2.45.2
2024-06-27T06:37:03.5281343Z ##[endgroup]
2024-06-27T06:37:03.5295242Z Temporarily overriding HOME='/home/runner/work/_temp/706df14b-b069-4b67-b73e-07f12134986d' before making global git config changes
2024-06-27T06:37:03.5296799Z Adding repository directory to the temporary git global config as a safe directory
2024-06-27T06:37:03.5300240Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/lazygit/lazygit
2024-06-27T06:37:03.5344066Z Deleting the contents of '/home/runner/work/lazygit/lazygit'
2024-06-27T06:37:03.5348418Z ##[group]Initializing the repository
2024-06-27T06:37:03.5351447Z [command]/usr/bin/git init /home/runner/work/lazygit/lazygit
2024-06-27T06:37:03.5466854Z hint: Using 'master' as the name for the initial branch. This default branch name
2024-06-27T06:37:03.5468051Z hint: is subject to change. To configure the initial branch name to use in all
2024-06-27T06:37:03.5468807Z hint: of your new repositories, which will suppress this warning, call:
2024-06-27T06:37:03.5469489Z hint:
2024-06-27T06:37:03.5470272Z hint: 	git config --global init.defaultBranch <name>
2024-06-27T06:37:03.5471007Z hint:
2024-06-27T06:37:03.5471663Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2024-06-27T06:37:03.5472449Z hint: 'development'. The just-created branch can be renamed via this command:
2024-06-27T06:37:03.5473025Z hint:
2024-06-27T06:37:03.5473405Z hint: 	git branch -m <name>
2024-06-27T06:37:03.5473967Z Initialized empty Git repository in /home/runner/work/lazygit/lazygit/.git/
2024-06-27T06:37:03.5480281Z [command]/usr/bin/git remote add origin https://github.com/jesseduffield/lazygit
2024-06-27T06:37:03.5525066Z ##[endgroup]
2024-06-27T06:37:03.5525958Z ##[group]Disabling automatic garbage collection
2024-06-27T06:37:03.5529928Z [command]/usr/bin/git config --local gc.auto 0
2024-06-27T06:37:03.5565106Z ##[endgroup]
2024-06-27T06:37:03.5565706Z ##[group]Setting up auth
2024-06-27T06:37:03.5570809Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2024-06-27T06:37:03.5606723Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2024-06-27T06:37:03.6020800Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2024-06-27T06:37:03.6057389Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2024-06-27T06:37:03.6299022Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2024-06-27T06:37:03.6342042Z ##[endgroup]
2024-06-27T06:37:03.6343079Z ##[group]Fetching the repository
2024-06-27T06:37:03.6352107Z [command]/usr/bin/git -c protocol.version=2 fetch --no-tags --prune --progress --no-recurse-submodules --depth=1 origin +63a523c2fcfac708c1c070cd4b550b4f41986555:refs/remotes/origin/master
2024-06-27T06:37:03.9960300Z remote: Enumerating objects: 2696, done.        
2024-06-27T06:37:03.9961968Z remote: Counting objects:   0% (1/2696)        
2024-06-27T06:37:03.9962871Z remote: Counting objects:   1% (27/2696)        
2024-06-27T06:37:03.9963890Z remote: Counting objects:   2% (54/2696)        
2024-06-27T06:37:03.9964768Z remote: Counting objects:   3% (81/2696)        
2024-06-27T06:37:03.9965622Z remote: Counting objects:   4% (108/2696)        
2024-06-27T06:37:03.9966468Z remote: Counting objects:   5% (135/2696)        
2024-06-27T06:37:03.9966932Z remote: Counting objects:   6% (162/2696)        
2024-06-27T06:37:03.9967446Z remote: Counting objects:   7% (189/2696)        
2024-06-27T06:37:03.9968032Z remote: Counting objects:   8% (216/2696)        
2024-06-27T06:37:03.9968517Z remote: Counting objects:   9% (243/2696)        
2024-06-27T06:37:03.9968967Z remote: Counting objects:  10% (270/2696)        
2024-06-27T06:37:03.9969527Z remote: Counting objects:  11% (297/2696)        
2024-06-27T06:37:03.9970011Z remote: Counting objects:  12% (324/2696)        
2024-06-27T06:37:03.9970443Z remote: Counting objects:  13% (351/2696)        
2024-06-27T06:37:03.9970978Z remote: Counting objects:  14% (378/2696)        
2024-06-27T06:37:03.9971457Z remote: Counting objects:  15% (405/2696)        
2024-06-27T06:37:03.9971912Z remote: Counting objects:  16% (432/2696)        
2024-06-27T06:37:03.9972516Z remote: Counting objects:  17% (459/2696)        
2024-06-27T06:37:03.9973005Z remote: Counting objects:  18% (486/2696)        
2024-06-27T06:37:03.9973695Z remote: Counting objects:  19% (513/2696)        
2024-06-27T06:37:03.9974203Z remote: Counting objects:  20% (540/2696)        
2024-06-27T06:37:03.9975033Z remote: Counting objects:  21% (567/2696)        
2024-06-27T06:37:03.9975525Z remote: Counting objects:  22% (594/2696)        
2024-06-27T06:37:03.9976036Z remote: Counting objects:  23% (621/2696)        
2024-06-27T06:37:03.9976542Z remote: Counting objects:  24% (648/2696)        
2024-06-27T06:37:03.9977022Z remote: Counting objects:  25% (674/2696)        
2024-06-27T06:37:03.9977576Z remote: Counting objects:  26% (701/2696)        
2024-06-27T06:37:03.9978005Z remote: Counting objects:  27% (728/2696)        
2024-06-27T06:37:03.9978476Z remote: Counting objects:  28% (755/2696)        
2024-06-27T06:37:03.9979031Z remote: Counting objects:  29% (782/2696)        
2024-06-27T06:37:03.9979460Z remote: Counting objects:  30% (809/2696)        
2024-06-27T06:37:03.9979950Z remote: Counting objects:  31% (836/2696)        
2024-06-27T06:37:03.9980520Z remote: Counting objects:  32% (863/2696)        
2024-06-27T06:37:03.9980961Z remote: Counting objects:  33% (890/2696)        
2024-06-27T06:37:03.9981522Z remote: Counting objects:  34% (917/2696)        
2024-06-27T06:37:03.9981994Z remote: Counting objects:  35% (944/2696)        
2024-06-27T06:37:03.9982560Z remote: Counting objects:  36% (971/2696)        
2024-06-27T06:37:03.9983025Z remote: Counting objects:  37% (998/2696)        
2024-06-27T06:37:03.9983505Z remote: Counting objects:  38% (1025/2696)        
2024-06-27T06:37:03.9984082Z remote: Counting objects:  39% (1052/2696)        
2024-06-27T06:37:03.9984546Z remote: Counting objects:  40% (1079/2696)        
2024-06-27T06:37:03.9985365Z remote: Counting objects:  41% (1106/2696)        
2024-06-27T06:37:03.9985973Z remote: Counting objects:  42% (1133/2696)        
2024-06-27T06:37:03.9986437Z remote: Counting objects:  43% (1160/2696)        
2024-06-27T06:37:03.9986918Z remote: Counting objects:  44% (1187/2696)        
2024-06-27T06:37:03.9987532Z remote: Counting objects:  45% (1214/2696)        
2024-06-27T06:37:03.9987983Z remote: Counting objects:  46% (1241/2696)        
2024-06-27T06:37:03.9988671Z remote: Counting objects:  47% (1268/2696)        
2024-06-27T06:37:03.9989316Z remote: Counting objects:  48% (1295/2696)        
2024-06-27T06:37:03.9989800Z remote: Counting objects:  49% (1322/2696)        
2024-06-27T06:37:03.9990349Z remote: Counting objects:  50% (1348/2696)        
2024-06-27T06:37:03.9990831Z remote: Counting objects:  51% (1375/2696)        
2024-06-27T06:37:03.9991311Z remote: Counting objects:  52% (1402/2696)        
2024-06-27T06:37:03.9991843Z remote: Counting objects:  53% (1429/2696)        
2024-06-27T06:37:03.9992358Z remote: Counting objects:  54% (1456/2696)        
2024-06-27T06:37:03.9992849Z remote: Counting objects:  55% (1483/2696)        
2024-06-27T06:37:03.9993555Z remote: Counting objects:  56% (1510/2696)        
2024-06-27T06:37:03.9994048Z remote: Counting objects:  57% (1537/2696)        
2024-06-27T06:37:03.9994616Z remote: Counting objects:  58% (1564/2696)        
2024-06-27T06:37:03.9995049Z remote: Counting objects:  59% (1591/2696)        
2024-06-27T06:37:03.9995621Z remote: Counting objects:  60% (1618/2696)        
2024-06-27T06:37:03.9996169Z remote: Counting objects:  61% (1645/2696)        
2024-06-27T06:37:03.9996642Z remote: Counting objects:  62% (1672/2696)        
2024-06-27T06:37:03.9997187Z remote: Counting objects:  63% (1699/2696)        
2024-06-27T06:37:03.9997758Z remote: Counting objects:  64% (1726/2696)        
2024-06-27T06:37:03.9998214Z remote: Counting objects:  65% (1753/2696)        
2024-06-27T06:37:03.9998773Z remote: Counting objects:  66% (1780/2696)        
2024-06-27T06:37:03.9999247Z remote: Counting objects:  67% (1807/2696)        
2024-06-27T06:37:03.9999701Z remote: Counting objects:  68% (1834/2696)        
2024-06-27T06:37:04.0000257Z remote: Counting objects:  69% (1861/2696)        
2024-06-27T06:37:04.0000871Z remote: Counting objects:  70% (1888/2696)        
2024-06-27T06:37:04.0001353Z remote: Counting objects:  71% (1915/2696)        
2024-06-27T06:37:04.0001933Z remote: Counting objects:  72% (1942/2696)        
2024-06-27T06:37:04.0002605Z remote: Counting objects:  73% (1969/2696)        
2024-06-27T06:37:04.0003050Z remote: Counting objects:  74% (1996/2696)        
2024-06-27T06:37:04.0239308Z remote: Counting objects:  75% (2022/2696)        
2024-06-27T06:37:04.0240304Z remote: Counting objects:  76% (2049/2696)        
2024-06-27T06:37:04.0240816Z remote: Counting objects:  77% (2076/2696)        
2024-06-27T06:37:04.0241324Z remote: Counting objects:  78% (2103/2696)        
2024-06-27T06:37:04.0241922Z remote: Counting objects:  79% (2130/2696)        
2024-06-27T06:37:04.0242381Z remote: Counting objects:  80% (2157/2696)        
2024-06-27T06:37:04.0242881Z remote: Counting objects:  81% (2184/2696)        
2024-06-27T06:37:04.0243472Z remote: Counting objects:  82% (2211/2696)        
2024-06-27T06:37:04.0243967Z remote: Counting objects:  83% (2238/2696)        
2024-06-27T06:37:04.0244441Z remote: Counting objects:  84% (2265/2696)        
2024-06-27T06:37:04.0245015Z remote: Counting objects:  85% (2292/2696)        
2024-06-27T06:37:04.0245508Z remote: Counting objects:  86% (2319/2696)        
2024-06-27T06:37:04.0245976Z remote: Counting objects:  87% (2346/2696)        
2024-06-27T06:37:04.0246537Z remote: Counting objects:  88% (2373/2696)        
2024-06-27T06:37:04.0247020Z remote: Counting objects:  89% (2400/2696)        
2024-06-27T06:37:04.0247486Z remote: Counting objects:  90% (2427/2696)        
2024-06-27T06:37:04.0248035Z remote: Counting objects:  91% (2454/2696)        
2024-06-27T06:37:04.0248520Z remote: Counting objects:  92% (2481/2696)        
2024-06-27T06:37:04.0248980Z remote: Counting objects:  93% (2508/2696)        
2024-06-27T06:37:04.0249523Z remote: Counting objects:  94% (2535/2696)        
2024-06-27T06:37:04.0250017Z remote: Counting objects:  95% (2562/2696)        
2024-06-27T06:37:04.0250457Z remote: Counting objects:  96% (2589/2696)        
2024-06-27T06:37:04.0250999Z remote: Counting objects:  97% (2616/2696)        
2024-06-27T06:37:04.0251498Z remote: Counting objects:  98% (2643/2696)        
2024-06-27T06:37:04.0252151Z remote: Counting objects:  99% (2670/2696)        
2024-06-27T06:37:04.0252777Z remote: Counting objects: 100% (2696/2696)        
2024-06-27T06:37:04.0253314Z remote: Counting objects: 100% (2696/2696), done.        
2024-06-27T06:37:04.0538812Z remote: Compressing objects:   0% (1/2259)        
2024-06-27T06:37:04.0539870Z remote: Compressing objects:   1% (23/2259)        
2024-06-27T06:37:04.0540599Z remote: Compressing objects:   2% (46/2259)        
2024-06-27T06:37:04.0541239Z remote: Compressing objects:   3% (68/2259)        
2024-06-27T06:37:04.0541935Z remote: Compressing objects:   4% (91/2259)        
2024-06-27T06:37:04.0542546Z remote: Compressing objects:   5% (113/2259)        
2024-06-27T06:37:04.0543057Z remote: Compressing objects:   6% (136/2259)        
2024-06-27T06:37:04.0543628Z remote: Compressing objects:   7% (159/2259)        
2024-06-27T06:37:04.0544134Z remote: Compressing objects:   8% (181/2259)        
2024-06-27T06:37:04.0544773Z remote: Compressing objects:   9% (204/2259)        
2024-06-27T06:37:04.0822355Z remote: Compressing objects:  10% (226/2259)        
2024-06-27T06:37:04.0823401Z remote: Compressing objects:  11% (249/2259)        
2024-06-27T06:37:04.0824587Z remote: Compressing objects:  12% (272/2259)        
2024-06-27T06:37:04.0825784Z remote: Compressing objects:  13% (294/2259)        
2024-06-27T06:37:04.0826774Z remote: Compressing objects:  14% (317/2259)        
2024-06-27T06:37:04.0827910Z remote: Compressing objects:  15% (339/2259)        
2024-06-27T06:37:04.0828844Z remote: Compressing objects:  16% (362/2259)        
2024-06-27T06:37:04.0829822Z remote: Compressing objects:  17% (385/2259)        
2024-06-27T06:37:04.0831002Z remote: Compressing objects:  18% (407/2259)        
2024-06-27T06:37:04.0831892Z remote: Compressing objects:  19% (430/2259)        
2024-06-27T06:37:04.0832813Z remote: Compressing objects:  20% (452/2259)        
2024-06-27T06:37:04.1402766Z remote: Compressing objects:  21% (475/2259)        
2024-06-27T06:37:04.1403817Z remote: Compressing objects:  22% (497/2259)        
2024-06-27T06:37:04.1404875Z remote: Compressing objects:  23% (520/2259)        
2024-06-27T06:37:04.1405777Z remote: Compressing objects:  24% (543/2259)        
2024-06-27T06:37:04.1406700Z remote: Compressing objects:  25% (565/2259)        
2024-06-27T06:37:04.1407672Z remote: Compressing objects:  26% (588/2259)        
2024-06-27T06:37:04.1408587Z remote: Compressing objects:  27% (610/2259)        
2024-06-27T06:37:04.1409547Z remote: Compressing objects:  28% (633/2259)        
2024-06-27T06:37:04.1410580Z remote: Compressing objects:  29% (656/2259)        
2024-06-27T06:37:04.1411497Z remote: Compressing objects:  30% (678/2259)        
2024-06-27T06:37:04.1412421Z remote: Compressing objects:  31% (701/2259)        
2024-06-27T06:37:04.1413409Z remote: Compressing objects:  32% (723/2259)        
2024-06-27T06:37:04.1414288Z remote: Compressing objects:  33% (746/2259)        
2024-06-27T06:37:04.1415271Z remote: Compressing objects:  34% (769/2259)        
2024-06-27T06:37:04.1416343Z remote: Compressing objects:  35% (791/2259)        
2024-06-27T06:37:04.1417337Z remote: Compressing objects:  36% (814/2259)        
2024-06-27T06:37:04.1418355Z remote: Compressing objects:  37% (836/2259)        
2024-06-27T06:37:04.2059031Z remote: Compressing objects:  38% (859/2259)        
2024-06-27T06:37:04.2060498Z remote: Compressing objects:  39% (882/2259)        
2024-06-27T06:37:04.2061251Z remote: Compressing objects:  40% (904/2259)        
2024-06-27T06:37:04.2061969Z remote: Compressing objects:  41% (927/2259)        
2024-06-27T06:37:04.2062796Z remote: Compressing objects:  42% (949/2259)        
2024-06-27T06:37:04.2063455Z remote: Compressing objects:  43% (972/2259)        
2024-06-27T06:37:04.2064144Z remote: Compressing objects:  44% (994/2259)        
2024-06-27T06:37:04.2065275Z remote: Compressing objects:  45% (1017/2259)        
2024-06-27T06:37:04.2065872Z remote: Compressing objects:  46% (1040/2259)        
2024-06-27T06:37:04.2066783Z remote: Compressing objects:  47% (1062/2259)        
2024-06-27T06:37:04.2067433Z remote: Compressing objects:  48% (1085/2259)        
2024-06-27T06:37:04.2067943Z remote: Compressing objects:  49% (1107/2259)        
2024-06-27T06:37:04.2068486Z remote: Compressing objects:  50% (1130/2259)        
2024-06-27T06:37:04.2069077Z remote: Compressing objects:  51% (1153/2259)        
2024-06-27T06:37:04.2069568Z remote: Compressing objects:  52% (1175/2259)        
2024-06-27T06:37:04.2070107Z remote: Compressing objects:  53% (1198/2259)        
2024-06-27T06:37:04.2070689Z remote: Compressing objects:  54% (1220/2259)        
2024-06-27T06:37:04.2071168Z remote: Compressing objects:  55% (1243/2259)        
2024-06-27T06:37:04.2071702Z remote: Compressing objects:  56% (1266/2259)        
2024-06-27T06:37:04.2072271Z remote: Compressing objects:  57% (1288/2259)        
2024-06-27T06:37:04.2557883Z remote: Compressing objects:  58% (1311/2259)        
2024-06-27T06:37:04.2558979Z remote: Compressing objects:  59% (1333/2259)        
2024-06-27T06:37:04.2562670Z remote: Compressing objects:  60% (1356/2259)        
2024-06-27T06:37:04.2563610Z remote: Compressing objects:  61% (1378/2259)        
2024-06-27T06:37:04.2564684Z remote: Compressing objects:  62% (1401/2259)        
2024-06-27T06:37:04.2565736Z remote: Compressing objects:  63% (1424/2259)        
2024-06-27T06:37:04.2566717Z remote: Compressing objects:  64% (1446/2259)        
2024-06-27T06:37:04.2567800Z remote: Compressing objects:  65% (1469/2259)        
2024-06-27T06:37:04.2568630Z remote: Compressing objects:  66% (1491/2259)        
2024-06-27T06:37:04.2569573Z remote: Compressing objects:  67% (1514/2259)        
2024-06-27T06:37:04.2570432Z remote: Compressing objects:  68% (1537/2259)        
2024-06-27T06:37:04.2571231Z remote: Compressing objects:  69% (1559/2259)        
2024-06-27T06:37:04.2572171Z remote: Compressing objects:  70% (1582/2259)        
2024-06-27T06:37:04.2573435Z remote: Compressing objects:  71% (1604/2259)        
2024-06-27T06:37:04.2574243Z remote: Compressing objects:  72% (1627/2259)        
2024-06-27T06:37:04.3071723Z remote: Compressing objects:  73% (1650/2259)        
2024-06-27T06:37:04.3072546Z remote: Compressing objects:  74% (1672/2259)        
2024-06-27T06:37:04.3073094Z remote: Compressing objects:  75% (1695/2259)        
2024-06-27T06:37:04.3073726Z remote: Compressing objects:  76% (1717/2259)        
2024-06-27T06:37:04.3653250Z remote: Compressing objects:  77% (1740/2259)        
2024-06-27T06:37:04.4028255Z remote: Compressing objects:  78% (1763/2259)        
2024-06-27T06:37:04.4029394Z remote: Compressing objects:  79% (1785/2259)        
2024-06-27T06:37:04.4032788Z remote: Compressing objects:  80% (1808/2259)        
2024-06-27T06:37:04.4033698Z remote: Compressing objects:  81% (1830/2259)        
2024-06-27T06:37:04.4034740Z remote: Compressing objects:  82% (1853/2259)        
2024-06-27T06:37:04.4035663Z remote: Compressing objects:  83% (1875/2259)        
2024-06-27T06:37:04.4036335Z remote: Compressing objects:  84% (1898/2259)        
2024-06-27T06:37:04.4037091Z remote: Compressing objects:  85% (1921/2259)        
2024-06-27T06:37:04.4037716Z remote: Compressing objects:  86% (1943/2259)        
2024-06-27T06:37:04.4038368Z remote: Compressing objects:  87% (1966/2259)        
2024-06-27T06:37:04.4039052Z remote: Compressing objects:  88% (1988/2259)        
2024-06-27T06:37:04.4039551Z remote: Compressing objects:  89% (2011/2259)        
2024-06-27T06:37:04.4040050Z remote: Compressing objects:  90% (2034/2259)        
2024-06-27T06:37:04.4040651Z remote: Compressing objects:  91% (2056/2259)        
2024-06-27T06:37:04.4041119Z remote: Compressing objects:  92% (2079/2259)        
2024-06-27T06:37:04.4041617Z remote: Compressing objects:  93% (2101/2259)        
2024-06-27T06:37:04.4042204Z remote: Compressing objects:  94% (2124/2259)        
2024-06-27T06:37:04.4042670Z remote: Compressing objects:  95% (2147/2259)        
2024-06-27T06:37:04.4043479Z remote: Compressing objects:  96% (2169/2259)        
2024-06-27T06:37:04.4044116Z remote: Compressing objects:  97% (2192/2259)        
2024-06-27T06:37:04.4047007Z remote: Compressing objects:  98% (2214/2259)        
2024-06-27T06:37:04.4049054Z remote: Compressing objects:  99% (2237/2259)        
2024-06-27T06:37:04.4050097Z remote: Compressing objects: 100% (2259/2259)        
2024-06-27T06:37:04.4051045Z remote: Compressing objects: 100% (2259/2259), done.        
2024-06-27T06:37:04.4232960Z Receiving objects:   0% (1/2696)
2024-06-27T06:37:04.4422061Z Receiving objects:   1% (27/2696)
2024-06-27T06:37:04.4631333Z Receiving objects:   2% (54/2696)
2024-06-27T06:37:04.4643910Z Receiving objects:   3% (81/2696)
2024-06-27T06:37:04.4655117Z Receiving objects:   4% (108/2696)
2024-06-27T06:37:04.4812526Z Receiving objects:   5% (135/2696)
2024-06-27T06:37:04.4819859Z Receiving objects:   6% (162/2696)
2024-06-27T06:37:04.4830478Z Receiving objects:   7% (189/2696)
2024-06-27T06:37:04.4838779Z Receiving objects:   8% (216/2696)
2024-06-27T06:37:04.4850234Z Receiving objects:   9% (243/2696)
2024-06-27T06:37:04.4862573Z Receiving objects:  10% (270/2696)
2024-06-27T06:37:04.4875175Z Receiving objects:  11% (297/2696)
2024-06-27T06:37:04.5000722Z Receiving objects:  12% (324/2696)
2024-06-27T06:37:04.5007683Z Receiving objects:  13% (351/2696)
2024-06-27T06:37:04.5018065Z Receiving objects:  14% (378/2696)
2024-06-27T06:37:04.5031177Z Receiving objects:  15% (405/2696)
2024-06-27T06:37:04.5037183Z Receiving objects:  16% (432/2696)
2024-06-27T06:37:04.5054178Z Receiving objects:  17% (459/2696)
2024-06-27T06:37:04.5080889Z Receiving objects:  18% (486/2696)
2024-06-27T06:37:04.5091111Z Receiving objects:  19% (513/2696)
2024-06-27T06:37:04.5096100Z Receiving objects:  20% (540/2696)
2024-06-27T06:37:04.5101285Z Receiving objects:  21% (567/2696)
2024-06-27T06:37:04.5104367Z Receiving objects:  22% (594/2696)
2024-06-27T06:37:04.5108652Z Receiving objects:  23% (621/2696)
2024-06-27T06:37:04.5114460Z Receiving objects:  24% (648/2696)
2024-06-27T06:37:04.5118783Z Receiving objects:  25% (674/2696)
2024-06-27T06:37:04.5123236Z Receiving objects:  26% (701/2696)
2024-06-27T06:37:04.5126632Z Receiving objects:  27% (728/2696)
2024-06-27T06:37:04.5129472Z Receiving objects:  28% (755/2696)
2024-06-27T06:37:04.5132808Z Receiving objects:  29% (782/2696)
2024-06-27T06:37:04.5180158Z Receiving objects:  30% (809/2696)
2024-06-27T06:37:04.5185851Z Receiving objects:  31% (836/2696)
2024-06-27T06:37:04.5192031Z Receiving objects:  32% (863/2696)
2024-06-27T06:37:04.5198594Z Receiving objects:  33% (890/2696)
2024-06-27T06:37:04.5207520Z Receiving objects:  34% (917/2696)
2024-06-27T06:37:04.5214964Z Receiving objects:  35% (944/2696)
2024-06-27T06:37:04.5220969Z Receiving objects:  36% (971/2696)
2024-06-27T06:37:04.5228643Z Receiving objects:  37% (998/2696)
2024-06-27T06:37:04.5235670Z Receiving objects:  38% (1025/2696)
2024-06-27T06:37:04.5240688Z Receiving objects:  39% (1052/2696)
2024-06-27T06:37:04.5248125Z Receiving objects:  40% (1079/2696)
2024-06-27T06:37:04.5254990Z Receiving objects:  41% (1106/2696)
2024-06-27T06:37:04.5269317Z Receiving objects:  42% (1133/2696)
2024-06-27T06:37:04.5275896Z Receiving objects:  43% (1160/2696)
2024-06-27T06:37:04.5278367Z Receiving objects:  44% (1187/2696)
2024-06-27T06:37:04.5281596Z Receiving objects:  45% (1214/2696)
2024-06-27T06:37:04.5287605Z Receiving objects:  46% (1241/2696)
2024-06-27T06:37:04.5296304Z Receiving objects:  47% (1268/2696)
2024-06-27T06:37:04.5301410Z Receiving objects:  48% (1295/2696)
2024-06-27T06:37:04.5307636Z Receiving objects:  49% (1322/2696)
2024-06-27T06:37:04.5311492Z Receiving objects:  50% (1348/2696)
2024-06-27T06:37:04.5322805Z Receiving objects:  51% (1375/2696)
2024-06-27T06:37:04.5335174Z Receiving objects:  52% (1402/2696)
2024-06-27T06:37:04.5342357Z Receiving objects:  53% (1429/2696)
2024-06-27T06:37:04.5350516Z Receiving objects:  54% (1456/2696)
2024-06-27T06:37:04.5362032Z Receiving objects:  55% (1483/2696)
2024-06-27T06:37:04.5372891Z Receiving objects:  56% (1510/2696)
2024-06-27T06:37:04.5387659Z Receiving objects:  57% (1537/2696)
2024-06-27T06:37:04.5395286Z Receiving objects:  58% (1564/2696)
2024-06-27T06:37:04.5409500Z Receiving objects:  59% (1591/2696)
2024-06-27T06:37:04.5418714Z Receiving objects:  60% (1618/2696)
2024-06-27T06:37:04.5426695Z Receiving objects:  61% (1645/2696)
2024-06-27T06:37:04.5441601Z Receiving objects:  62% (1672/2696)
2024-06-27T06:37:04.5451612Z Receiving objects:  63% (1699/2696)
2024-06-27T06:37:04.5489512Z Receiving objects:  64% (1726/2696)
2024-06-27T06:37:04.5636680Z Receiving objects:  65% (1753/2696)
2024-06-27T06:37:04.5645009Z Receiving objects:  66% (1780/2696)
2024-06-27T06:37:04.5651340Z Receiving objects:  67% (1807/2696)
2024-06-27T06:37:04.5685935Z Receiving objects:  68% (1834/2696)
2024-06-27T06:37:04.5725683Z Receiving objects:  69% (1861/2696)
2024-06-27T06:37:04.5737569Z Receiving objects:  70% (1888/2696)
2024-06-27T06:37:04.5748415Z Receiving objects:  71% (1915/2696)
2024-06-27T06:37:04.5757132Z Receiving objects:  72% (1942/2696)
2024-06-27T06:37:04.5766059Z Receiving objects:  73% (1969/2696)
2024-06-27T06:37:04.5771730Z Receiving objects:  74% (1996/2696)
2024-06-27T06:37:04.5781505Z Receiving objects:  75% (2022/2696)
2024-06-27T06:37:04.5798562Z Receiving objects:  76% (2049/2696)
2024-06-27T06:37:04.5805210Z Receiving objects:  77% (2076/2696)
2024-06-27T06:37:04.5815562Z Receiving objects:  78% (2103/2696)
2024-06-27T06:37:04.5836502Z Receiving objects:  79% (2130/2696)
2024-06-27T06:37:04.5857668Z Receiving objects:  80% (2157/2696)
2024-06-27T06:37:04.5865951Z Receiving objects:  81% (2184/2696)
2024-06-27T06:37:04.5871288Z Receiving objects:  82% (2211/2696)
2024-06-27T06:37:04.5876417Z Receiving objects:  83% (2238/2696)
2024-06-27T06:37:04.5881745Z Receiving objects:  84% (2265/2696)
2024-06-27T06:37:04.5891028Z Receiving objects:  85% (2292/2696)
2024-06-27T06:37:04.5897792Z Receiving objects:  86% (2319/2696)
2024-06-27T06:37:04.5906175Z Receiving objects:  87% (2346/2696)
2024-06-27T06:37:04.5931225Z Receiving objects:  88% (2373/2696)
2024-06-27T06:37:04.5940740Z Receiving objects:  89% (2400/2696)
2024-06-27T06:37:04.6022147Z Receiving objects:  90% (2427/2696)
2024-06-27T06:37:04.6058330Z Receiving objects:  91% (2454/2696)
2024-06-27T06:37:04.6081450Z Receiving objects:  92% (2481/2696)
2024-06-27T06:37:04.6116037Z Receiving objects:  93% (2508/2696)
2024-06-27T06:37:04.6140114Z Receiving objects:  94% (2535/2696)
2024-06-27T06:37:04.6179367Z Receiving objects:  95% (2562/2696)
2024-06-27T06:37:04.6193367Z Receiving objects:  96% (2589/2696)
2024-06-27T06:37:04.6425366Z Receiving objects:  97% (2616/2696)
2024-06-27T06:37:04.7329036Z Receiving objects:  98% (2643/2696)
2024-06-27T06:37:04.7440323Z Receiving objects:  99% (2670/2696)
2024-06-27T06:37:04.7442244Z remote: Total 2696 (delta 476), reused 1423 (delta 244), pack-reused 0        
2024-06-27T06:37:04.7443328Z Receiving objects: 100% (2696/2696)
2024-06-27T06:37:04.7444142Z Receiving objects: 100% (2696/2696), 4.74 MiB | 14.07 MiB/s, done.
2024-06-27T06:37:04.7454339Z Resolving deltas:   0% (0/476)
2024-06-27T06:37:04.7458602Z Resolving deltas:   1% (5/476)
2024-06-27T06:37:04.7462377Z Resolving deltas:   2% (10/476)
2024-06-27T06:37:04.7463955Z Resolving deltas:   3% (15/476)
2024-06-27T06:37:04.7464632Z Resolving deltas:   4% (20/476)
2024-06-27T06:37:04.7468146Z Resolving deltas:   5% (24/476)
2024-06-27T06:37:04.7471960Z Resolving deltas:   6% (29/476)
2024-06-27T06:37:04.7473518Z Resolving deltas:   7% (34/476)
2024-06-27T06:37:04.7476932Z Resolving deltas:   8% (39/476)
2024-06-27T06:37:04.7479235Z Resolving deltas:   9% (43/476)
2024-06-27T06:37:04.7479998Z Resolving deltas:  10% (49/476)
2024-06-27T06:37:04.7480689Z Resolving deltas:  11% (53/476)
2024-06-27T06:37:04.7482839Z Resolving deltas:  12% (58/476)
2024-06-27T06:37:04.7483642Z Resolving deltas:  13% (62/476)
2024-06-27T06:37:04.7484367Z Resolving deltas:  14% (67/476)
2024-06-27T06:37:04.7485216Z Resolving deltas:  15% (72/476)
2024-06-27T06:37:04.7486279Z Resolving deltas:  16% (77/476)
2024-06-27T06:37:04.7487070Z Resolving deltas:  17% (81/476)
2024-06-27T06:37:04.7487929Z Resolving deltas:  18% (86/476)
2024-06-27T06:37:04.7488677Z Resolving deltas:  19% (91/476)
2024-06-27T06:37:04.7489378Z Resolving deltas:  20% (96/476)
2024-06-27T06:37:04.7490120Z Resolving deltas:  21% (100/476)
2024-06-27T06:37:04.7490867Z Resolving deltas:  22% (105/476)
2024-06-27T06:37:04.7491611Z Resolving deltas:  23% (110/476)
2024-06-27T06:37:04.7492425Z Resolving deltas:  24% (115/476)
2024-06-27T06:37:04.7493036Z Resolving deltas:  25% (119/476)
2024-06-27T06:37:04.7493685Z Resolving deltas:  26% (124/476)
2024-06-27T06:37:04.7494792Z Resolving deltas:  27% (129/476)
2024-06-27T06:37:04.7495753Z Resolving deltas:  28% (134/476)
2024-06-27T06:37:04.7496760Z Resolving deltas:  29% (139/476)
2024-06-27T06:37:04.7497931Z Resolving deltas:  30% (143/476)
2024-06-27T06:37:04.7500190Z Resolving deltas:  31% (148/476)
2024-06-27T06:37:04.7503964Z Resolving deltas:  32% (153/476)
2024-06-27T06:37:04.7505122Z Resolving deltas:  33% (158/476)
2024-06-27T06:37:04.7505814Z Resolving deltas:  34% (162/476)
2024-06-27T06:37:04.7506555Z Resolving deltas:  35% (168/476)
2024-06-27T06:37:04.7507476Z Resolving deltas:  36% (172/476)
2024-06-27T06:37:04.7508222Z Resolving deltas:  37% (177/476)
2024-06-27T06:37:04.7508888Z Resolving deltas:  38% (182/476)
2024-06-27T06:37:04.7509887Z Resolving deltas:  39% (186/476)
2024-06-27T06:37:04.7512123Z Resolving deltas:  40% (191/476)
2024-06-27T06:37:04.7515197Z Resolving deltas:  41% (196/476)
2024-06-27T06:37:04.7516146Z Resolving deltas:  42% (200/476)
2024-06-27T06:37:04.7516929Z Resolving deltas:  43% (205/476)
2024-06-27T06:37:04.7517626Z Resolving deltas:  44% (210/476)
2024-06-27T06:37:04.7518519Z Resolving deltas:  45% (215/476)
2024-06-27T06:37:04.7519182Z Resolving deltas:  46% (220/476)
2024-06-27T06:37:04.7519861Z Resolving deltas:  47% (224/476)
2024-06-27T06:37:04.7521047Z Resolving deltas:  48% (229/476)
2024-06-27T06:37:04.7521810Z Resolving deltas:  49% (235/476)
2024-06-27T06:37:04.7523057Z Resolving deltas:  50% (238/476)
2024-06-27T06:37:04.7525952Z Resolving deltas:  51% (243/476)
2024-06-27T06:37:04.7526625Z Resolving deltas:  52% (248/476)
2024-06-27T06:37:04.7527433Z Resolving deltas:  53% (253/476)
2024-06-27T06:37:04.7528026Z Resolving deltas:  54% (258/476)
2024-06-27T06:37:04.7528695Z Resolving deltas:  55% (262/476)
2024-06-27T06:37:04.7531841Z Resolving deltas:  56% (267/476)
2024-06-27T06:37:04.7533939Z Resolving deltas:  57% (272/476)
2024-06-27T06:37:04.7535397Z Resolving deltas:  58% (277/476)
2024-06-27T06:37:04.7537174Z Resolving deltas:  59% (281/476)
2024-06-27T06:37:04.7538052Z Resolving deltas:  60% (286/476)
2024-06-27T06:37:04.7540871Z Resolving deltas:  61% (291/476)
2024-06-27T06:37:04.7545980Z Resolving deltas:  62% (296/476)
2024-06-27T06:37:04.7546660Z Resolving deltas:  63% (300/476)
2024-06-27T06:37:04.7547300Z Resolving deltas:  64% (305/476)
2024-06-27T06:37:04.7552266Z Resolving deltas:  65% (310/476)
2024-06-27T06:37:04.7557251Z Resolving deltas:  66% (315/476)
2024-06-27T06:37:04.7558156Z Resolving deltas:  67% (319/476)
2024-06-27T06:37:04.7559126Z Resolving deltas:  68% (324/476)
2024-06-27T06:37:04.7564317Z Resolving deltas:  69% (329/476)
2024-06-27T06:37:04.7564993Z Resolving deltas:  70% (334/476)
2024-06-27T06:37:04.7565785Z Resolving deltas:  71% (338/476)
2024-06-27T06:37:04.7566422Z Resolving deltas:  72% (343/476)
2024-06-27T06:37:04.7567061Z Resolving deltas:  73% (348/476)
2024-06-27T06:37:04.7569358Z Resolving deltas:  74% (353/476)
2024-06-27T06:37:04.7571308Z Resolving deltas:  75% (357/476)
2024-06-27T06:37:04.7575252Z Resolving deltas:  76% (362/476)
2024-06-27T06:37:04.7580492Z Resolving deltas:  77% (367/476)
2024-06-27T06:37:04.7581395Z Resolving deltas:  78% (372/476)
2024-06-27T06:37:04.7581988Z Resolving deltas:  79% (377/476)
2024-06-27T06:37:04.7587637Z Resolving deltas:  80% (381/476)
2024-06-27T06:37:04.7596989Z Resolving deltas:  81% (386/476)
2024-06-27T06:37:04.7608307Z Resolving deltas:  82% (391/476)
2024-06-27T06:37:04.7617804Z Resolving deltas:  83% (396/476)
2024-06-27T06:37:04.7627921Z Resolving deltas:  84% (400/476)
2024-06-27T06:37:04.7635687Z Resolving deltas:  85% (405/476)
2024-06-27T06:37:04.7643645Z Resolving deltas:  86% (410/476)
2024-06-27T06:37:04.7648057Z Resolving deltas:  87% (416/476)
2024-06-27T06:37:04.7652600Z Resolving deltas:  88% (419/476)
2024-06-27T06:37:04.7658232Z Resolving deltas:  89% (424/476)
2024-06-27T06:37:04.7662110Z Resolving deltas:  90% (429/476)
2024-06-27T06:37:04.7667344Z Resolving deltas:  91% (434/476)
2024-06-27T06:37:04.7668184Z Resolving deltas:  92% (439/476)
2024-06-27T06:37:04.7671439Z Resolving deltas:  93% (443/476)
2024-06-27T06:37:04.7673686Z Resolving deltas:  94% (448/476)
2024-06-27T06:37:04.7677929Z Resolving deltas:  95% (454/476)
2024-06-27T06:37:04.7682413Z Resolving deltas:  96% (458/476)
2024-06-27T06:37:04.7683124Z Resolving deltas:  97% (462/476)
2024-06-27T06:37:04.7715818Z Resolving deltas:  98% (467/476)
2024-06-27T06:37:04.7801582Z Resolving deltas:  99% (472/476)
2024-06-27T06:37:04.7803245Z Resolving deltas: 100% (476/476)
2024-06-27T06:37:04.7803666Z Resolving deltas: 100% (476/476), done.
2024-06-27T06:37:04.7976432Z From https://github.com/jesseduffield/lazygit
2024-06-27T06:37:04.7977526Z  * [new ref]         63a523c2fcfac708c1c070cd4b550b4f41986555 -> origin/master
2024-06-27T06:37:04.8003937Z ##[endgroup]
2024-06-27T06:37:04.8004861Z ##[group]Determining the checkout info
2024-06-27T06:37:04.8006269Z ##[endgroup]
2024-06-27T06:37:04.8007140Z ##[group]Checking out the ref
2024-06-27T06:37:04.8013764Z [command]/usr/bin/git checkout --progress --force -B master refs/remotes/origin/master
2024-06-27T06:37:04.9786288Z Reset branch 'master'
2024-06-27T06:37:04.9787815Z branch 'master' set up to track 'origin/master'.
2024-06-27T06:37:04.9802522Z ##[endgroup]
2024-06-27T06:37:04.9851995Z [command]/usr/bin/git log -1 --format='%H'
2024-06-27T06:37:04.9883087Z '63a523c2fcfac708c1c070cd4b550b4f41986555'
2024-06-27T06:37:05.0179506Z ##[group]Run actions/setup-go@v4
2024-06-27T06:37:05.0179922Z with:
2024-06-27T06:37:05.0180327Z   go-version: 1.22.x
2024-06-27T06:37:05.0180705Z   check-latest: false
2024-06-27T06:37:05.0181171Z   token: ***
2024-06-27T06:37:05.0181577Z   cache: true
2024-06-27T06:37:05.0181898Z env:
2024-06-27T06:37:05.0182151Z   GO_VERSION: 1.22
2024-06-27T06:37:05.0182555Z   GOFLAGS: -mod=vendor
2024-06-27T06:37:05.0182913Z   GOARCH: amd64
2024-06-27T06:37:05.0183194Z ##[endgroup]
2024-06-27T06:37:05.1428358Z Setup go version spec 1.22.x
2024-06-27T06:37:05.1475707Z Found in cache @ /opt/hostedtoolcache/go/1.22.4/x64
2024-06-27T06:37:05.1483932Z Added go to the path
2024-06-27T06:37:05.1487953Z Successfully set up Go version 1.22.x
2024-06-27T06:37:05.2050329Z [command]/opt/hostedtoolcache/go/1.22.4/x64/bin/go env GOMODCACHE
2024-06-27T06:37:05.2092736Z [command]/opt/hostedtoolcache/go/1.22.4/x64/bin/go env GOCACHE
2024-06-27T06:37:05.2129387Z /home/runner/go/pkg/mod
2024-06-27T06:37:05.2149552Z /home/runner/.cache/go-build
2024-06-27T06:37:06.8632189Z Received 0 of 284707931 (0.0%), 0.0 MBs/sec
2024-06-27T06:37:07.8633050Z Received 104857600 of 284707931 (36.8%), 50.0 MBs/sec
2024-06-27T06:37:08.8635508Z Received 180355072 of 284707931 (63.3%), 57.3 MBs/sec
2024-06-27T06:37:09.8644289Z Received 268435456 of 284707931 (94.3%), 64.0 MBs/sec
2024-06-27T06:37:10.0216979Z Received 284707931 of 284707931 (100.0%), 65.3 MBs/sec
2024-06-27T06:37:10.0218467Z Cache Size: ~272 MB (284707931 B)
2024-06-27T06:37:10.0253546Z [command]/usr/bin/tar -xf /home/runner/work/_temp/a465853f-8010-4add-8547-bf8c6306605a/cache.tzst -P -C /home/runner/work/lazygit/lazygit --use-compress-program unzstd
2024-06-27T06:37:11.5100202Z Cache restored successfully
2024-06-27T06:37:11.5652781Z Cache restored from key: setup-go-Linux-ubuntu22-go-1.22.4-9f8bf866b5b460401df4751f1b30452d7ee57e2dc76fa4ebfa6deac9733dae58
2024-06-27T06:37:11.5681273Z go version go1.22.4 linux/amd64
2024-06-27T06:37:11.5681585Z 
2024-06-27T06:37:11.5682036Z ##[group]go env
2024-06-27T06:37:11.5809190Z GO111MODULE=''
2024-06-27T06:37:11.5809778Z GOARCH='amd64'
2024-06-27T06:37:11.5810252Z GOBIN=''
2024-06-27T06:37:11.5810625Z GOCACHE='/home/runner/.cache/go-build'
2024-06-27T06:37:11.5811138Z GOENV='/home/runner/.config/go/env'
2024-06-27T06:37:11.5811634Z GOEXE=''
2024-06-27T06:37:11.5812047Z GOEXPERIMENT=''
2024-06-27T06:37:11.5812453Z GOFLAGS='-mod=vendor'
2024-06-27T06:37:11.5812949Z GOHOSTARCH='amd64'
2024-06-27T06:37:11.5813342Z GOHOSTOS='linux'
2024-06-27T06:37:11.5813692Z GOINSECURE=''
2024-06-27T06:37:11.5814157Z GOMODCACHE='/home/runner/go/pkg/mod'
2024-06-27T06:37:11.5814578Z GONOPROXY=''
2024-06-27T06:37:11.5814911Z GONOSUMDB=''
2024-06-27T06:37:11.5815311Z GOOS='linux'
2024-06-27T06:37:11.5815677Z GOPATH='/home/runner/go'
2024-06-27T06:37:11.5816116Z GOPRIVATE=''
2024-06-27T06:37:11.5816529Z GOPROXY='https://proxy.golang.org,direct'
2024-06-27T06:37:11.5817075Z GOROOT='/opt/hostedtoolcache/go/1.22.4/x64'
2024-06-27T06:37:11.5817668Z GOSUMDB='sum.golang.org'
2024-06-27T06:37:11.5818059Z GOTMPDIR=''
2024-06-27T06:37:11.5818368Z GOTOOLCHAIN='auto'
2024-06-27T06:37:11.5818982Z GOTOOLDIR='/opt/hostedtoolcache/go/1.22.4/x64/pkg/tool/linux_amd64'
2024-06-27T06:37:11.5819554Z GOVCS=''
2024-06-27T06:37:11.5819891Z GOVERSION='go1.22.4'
2024-06-27T06:37:11.5820336Z GCCGO='gccgo'
2024-06-27T06:37:11.5820643Z GOAMD64='v1'
2024-06-27T06:37:11.5820969Z AR='ar'
2024-06-27T06:37:11.5821363Z CC='gcc'
2024-06-27T06:37:11.5821675Z CXX='g++'
2024-06-27T06:37:11.5822029Z CGO_ENABLED='1'
2024-06-27T06:37:11.5822512Z GOMOD='/home/runner/work/lazygit/lazygit/go.mod'
2024-06-27T06:37:11.5822989Z GOWORK=''
2024-06-27T06:37:11.5823346Z CGO_CFLAGS='-O2 -g'
2024-06-27T06:37:11.5823764Z CGO_CPPFLAGS=''
2024-06-27T06:37:11.5824124Z CGO_CXXFLAGS='-O2 -g'
2024-06-27T06:37:11.5824488Z CGO_FFLAGS='-O2 -g'
2024-06-27T06:37:11.5825223Z CGO_LDFLAGS='-O2 -g'
2024-06-27T06:37:11.5825736Z PKG_CONFIG='pkg-config'
2024-06-27T06:37:11.5827368Z GOGCCFLAGS='-fPIC -m64 -pthread -Wl,--no-gc-sections -fmessage-length=0 -ffile-prefix-map=/tmp/go-build1725696872=/tmp/go-build -gno-record-gcc-switches'
2024-06-27T06:37:11.5828156Z 
2024-06-27T06:37:11.5828689Z ##[endgroup]
2024-06-27T06:37:11.6006350Z ##[group]Run go mod vendor && git diff --exit-code || (echo "Unexpected change to vendor directory. Run 'go mod vendor' locally and commit the changes" && exit 1)
2024-06-27T06:37:11.6007889Z [36;1mgo mod vendor && git diff --exit-code || (echo "Unexpected change to vendor directory. Run 'go mod vendor' locally and commit the changes" && exit 1)[0m
2024-06-27T06:37:11.6194151Z shell: /usr/bin/bash -e {0}
2024-06-27T06:37:11.6194543Z env:
2024-06-27T06:37:11.6195083Z   GO_VERSION: 1.22
2024-06-27T06:37:11.6195450Z   GOFLAGS: -mod=vendor
2024-06-27T06:37:11.6195806Z   GOARCH: amd64
2024-06-27T06:37:11.6196199Z ##[endgroup]
2024-06-27T06:37:12.1222487Z ##[group]Run go mod tidy && git diff --exit-code || (echo "go.mod file is not clean. Run 'go mod tidy' locally and commit the changes" && exit 1)
2024-06-27T06:37:12.1223778Z [36;1mgo mod tidy && git diff --exit-code || (echo "go.mod file is not clean. Run 'go mod tidy' locally and commit the changes" && exit 1)[0m
2024-06-27T06:37:12.1284567Z shell: /usr/bin/bash -e {0}
2024-06-27T06:37:12.1284927Z env:
2024-06-27T06:37:12.1285335Z   GO_VERSION: 1.22
2024-06-27T06:37:12.1285696Z   GOFLAGS: -mod=vendor
2024-06-27T06:37:12.1286045Z   GOARCH: amd64
2024-06-27T06:37:12.1286414Z ##[endgroup]
2024-06-27T06:37:12.2182747Z ##[group]Run go generate ./... && git diff --quiet || (git status -s; echo "Auto-generated files not up to date. Run 'go generate ./...' locally and commit the changes" && exit 1)
2024-06-27T06:37:12.2184422Z [36;1mgo generate ./... && git diff --quiet || (git status -s; echo "Auto-generated files not up to date. Run 'go generate ./...' locally and commit the changes" && exit 1)[0m
2024-06-27T06:37:12.2248246Z shell: /usr/bin/bash --noprofile --norc -e -o pipefail {0}
2024-06-27T06:37:12.2248904Z env:
2024-06-27T06:37:12.2249230Z   GO_VERSION: 1.22
2024-06-27T06:37:12.2249648Z   GOFLAGS: -mod=vendor
2024-06-27T06:37:12.2249998Z   GOARCH: amd64
2024-06-27T06:37:12.2250304Z ##[endgroup]
2024-06-27T06:37:19.9721651Z Generating cheatsheets in /home/runner/work/lazygit/lazygit/docs/keybindings...
2024-06-27T06:37:20.1842673Z Generating test_list.go...
2024-06-27T06:37:20.4287982Z Generating jsonschema in /home/runner/work/lazygit/lazygit/schema...
2024-06-27T06:37:20.4597693Z ##[group]Run scripts/check_filenames.sh
2024-06-27T06:37:20.4598560Z [36;1mscripts/check_filenames.sh[0m
2024-06-27T06:37:20.4662342Z shell: /usr/bin/bash -e {0}
2024-06-27T06:37:20.4662864Z env:
2024-06-27T06:37:20.4663184Z   GO_VERSION: 1.22
2024-06-27T06:37:20.4663536Z   GOFLAGS: -mod=vendor
2024-06-27T06:37:20.4663942Z   GOARCH: amd64
2024-06-27T06:37:20.4664270Z ##[endgroup]
2024-06-27T06:37:20.4923943Z All Go files in the project (excluding vendor directory) use lowercase letters
2024-06-27T06:37:20.4979461Z Post job cleanup.
2024-06-27T06:37:20.6211116Z [command]/opt/hostedtoolcache/go/1.22.4/x64/bin/go env GOMODCACHE
2024-06-27T06:37:20.6259106Z [command]/opt/hostedtoolcache/go/1.22.4/x64/bin/go env GOCACHE
2024-06-27T06:37:20.6292781Z /home/runner/go/pkg/mod
2024-06-27T06:37:20.6316936Z /home/runner/.cache/go-build
2024-06-27T06:37:20.6322446Z Cache hit occurred on the primary key setup-go-Linux-ubuntu22-go-1.22.4-9f8bf866b5b460401df4751f1b30452d7ee57e2dc76fa4ebfa6deac9733dae58, not saving cache.
2024-06-27T06:37:20.6442880Z Post job cleanup.
2024-06-27T06:37:20.7268292Z [command]/usr/bin/git version
2024-06-27T06:37:20.7312116Z git version 2.45.2
2024-06-27T06:37:20.7350237Z Temporarily overriding HOME='/home/runner/work/_temp/95ae4e5b-b3d2-46c4-8624-4eb1fcf9d9a9' before making global git config changes
2024-06-27T06:37:20.7351843Z Adding repository directory to the temporary git global config as a safe directory
2024-06-27T06:37:20.7355822Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/lazygit/lazygit
2024-06-27T06:37:20.7396825Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2024-06-27T06:37:20.7434570Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2024-06-27T06:37:20.7679051Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2024-06-27T06:37:20.7706552Z http.https://github.com/.extraheader
2024-06-27T06:37:20.7717504Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2024-06-27T06:37:20.7755581Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2024-06-27T06:37:20.8207808Z Cleaning up orphan processes**
