node{
    stage 'Github Polling'
        git 'https://github.com/debabratamca/JenkinsTestWindows.git'
    stage 'Nuget Packages Restore'
        bat label: '', script:'''"D:\\Software\\Automation\\nuget.exe" restore "C:\\Program Files (x86)\\Jenkins\\jobs\\MSBuildINGithubPipeline\\workspace\\JenkinsTestWindows.sln"'''
    stage 'Buiild MSBuild'
        bat label: '', script: '''set msbildpath="C:\\Program Files (x86)\\Microsoft Visual Studio\\2019\\Community\\MSBuild\\Current\\Bin\\"
        cd %msbildpath%
        MSBuild.exe "C:\\Program Files (x86)\\Jenkins\\jobs\\MSBuildINGithubPipeline\\workspace\\JenkinsTestWindows.sln"'''
}