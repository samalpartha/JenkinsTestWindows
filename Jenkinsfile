node{
    stage 'Github Polling'
        git 'https://github.com/samalpartha/JenkinsTestWindows.git'
    stage 'Nuget Packages Restore'
        bat label: '', script:'''"C:\\Users\\Partha\\Documents\\nuget.exe restore "C:\\Program Files (x86)\\Jenkins\\workspace\\JenkinsTestWindows\\JenkinsTestWindows.sln"'''
    stage 'Buiild MSBuild'
        bat label: '', script: '''set msbildpath="C:\\Program Files (x86)\\Microsoft Visual Studio\\2019\\Community\\MSBuild\\Current\\Bin\\"
        cd %msbildpath%
        MSBuild.exe "C:\\Program Files (x86)\\Jenkins\\workspace\\JenkinsTestWindows\\JenkinsTestWindows.sln"'''
		}
