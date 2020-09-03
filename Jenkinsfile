pipeline {
    agent any
    
        
    
    stages{
        stage('Deploy-Case01')
        {
            when{
                allOf {
                    expression{params.Actions == 'Deploy'}
                    expression{params.Environment == 'QA'}
                    expression{params.Branch == 'master'} 
                    
                    }
                
            }
            steps{
                println ('Deploy - QA - Master');
            }
        }
        stage('Deploy-Case02')
        {
           when{
                allOf {
                    expression{params.Actions == 'Deploy'}
                
                    expression{params.Environment == 'Dev'}
                    expression{params.Environment == 'QA'}
                    expression{params.Environment == 'Prod'}
                    expression{params.Branch == 'master'} 
                    }
            }
            steps{
                println ('Deploy - Dev - master');
            }
        }
        stage('Deploy-Case03')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Deploy'}
                    expression{params.Environment == 'Prod'}
                    expression{params.Branch == 'master'} 
                    }
            }
            steps{
                println ('Deploy - Prod - Master');
            }
        }
        
        
        
        stage('Promote-Case01')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Promote'}
                    expression{params.Environment == 'Dev'}
                    expression{params.Branch == 'Dev'}
                    }
            }
            steps{
               //git branch: 'develop', credentialsId: 'privateKey', url: 'gitea@git.we-support.se:Trapeze/TrapezeCommon.git'
               
               //bat """ "C:/Program Files (x86)/IIS/Microsoft Web Deploy V3/msdeploy.exe" -verb=sync -source:contentPath="D:\\try02" -dest:auto,computerName=https://CRLHS-PNMS07:8172/msdeploy.axd?site=TestSite,username="CONTOURSOFTWARE\\rehmayas",password="rehmayas1",authType="Basic" -enableRule:DoNotDeleteRule -enablerule:AppOffline -setParam:value="TestSite",kind=ProviderPath,scope=contentPath -AllowUntrusted="True" """
            
                println('Promote - Dev - Dev');
            }
        }
        
        stage('Promote-Case02')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Promote'}
                    expression{params.Environment == 'QA'}
                    expression{params.Branch == 'Dev'}
                    }
            }
            steps{
               //git branch: 'develop', credentialsId: 'privateKey', url: 'gitea@git.we-support.se:Trapeze/TrapezeCommon.git'
               
               //bat """ "C:/Program Files (x86)/IIS/Microsoft Web Deploy V3/msdeploy.exe" -verb=sync -source:contentPath="D:\\try02" -dest:auto,computerName=https://CRLHS-PNMS07:8172/msdeploy.axd?site=TestSite,username="CONTOURSOFTWARE\\rehmayas",password="rehmayas1",authType="Basic" -enableRule:DoNotDeleteRule -enablerule:AppOffline -setParam:value="TestSite",kind=ProviderPath,scope=contentPath -AllowUntrusted="True" """
            
                println('Promote - QA - Dev');
            }
        }
        stage('Promote-Case03')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Promote'}
                    expression{params.Environment == 'Prod'}
                    expression{params.Branch == 'Dev'}
                    }
            }
            steps{
               //git branch: 'develop', credentialsId: 'privateKey', url: 'gitea@git.we-support.se:Trapeze/TrapezeCommon.git'
               
               //bat """ "C:/Program Files (x86)/IIS/Microsoft Web Deploy V3/msdeploy.exe" -verb=sync -source:contentPath="D:\\try02" -dest:auto,computerName=https://CRLHS-PNMS07:8172/msdeploy.axd?site=TestSite,username="CONTOURSOFTWARE\\rehmayas",password="rehmayas1",authType="Basic" -enableRule:DoNotDeleteRule -enablerule:AppOffline -setParam:value="TestSite",kind=ProviderPath,scope=contentPath -AllowUntrusted="True" """
            
                println('Promote - Prod - Dev');
            }
        }
        
        stage('Rollback-Case01')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Rollback'}
                    expression{params.Environment == 'Dev'}
                    expression{params.Branch == 'Dev'}
                    }
            }
            steps{
               //git branch: 'develop', credentialsId: 'privateKey', url: 'gitea@git.we-support.se:Trapeze/TrapezeCommon.git'
               
               //bat """ "C:/Program Files (x86)/IIS/Microsoft Web Deploy V3/msdeploy.exe" -verb=sync -source:contentPath="D:\\try02" -dest:auto,computerName=https://CRLHS-PNMS07:8172/msdeploy.axd?site=TestSite,username="CONTOURSOFTWARE\\rehmayas",password="rehmayas1",authType="Basic" -enableRule:DoNotDeleteRule -enablerule:AppOffline -setParam:value="TestSite",kind=ProviderPath,scope=contentPath -AllowUntrusted="True" """
            
                println('Rollback - Dev - Dev');
            }
        }
        stage('Rollback-Case02')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Rollback'}
                    expression{params.Environment == 'QA'}
                    expression{params.Branch == 'Dev'}
                    }
            }
            steps{
               //git branch: 'develop', credentialsId: 'privateKey', url: 'gitea@git.we-support.se:Trapeze/TrapezeCommon.git'
               
               //bat """ "C:/Program Files (x86)/IIS/Microsoft Web Deploy V3/msdeploy.exe" -verb=sync -source:contentPath="D:\\try02" -dest:auto,computerName=https://CRLHS-PNMS07:8172/msdeploy.axd?site=TestSite,username="CONTOURSOFTWARE\\rehmayas",password="rehmayas1",authType="Basic" -enableRule:DoNotDeleteRule -enablerule:AppOffline -setParam:value="TestSite",kind=ProviderPath,scope=contentPath -AllowUntrusted="True" """
            
                println('Rollback - QA - Dev');
            }
        }
        stage('Rollback-Case03')
        {
            when{
                 allOf {
                    expression{params.Actions == 'Rollback'}
                    expression{params.Environment == 'Prod'}
                    expression{params.Branch == 'Dev'}
                    }
            }
            steps{
               //git branch: 'develop', credentialsId: 'privateKey', url: 'gitea@git.we-support.se:Trapeze/TrapezeCommon.git'
               
               //bat """ "C:/Program Files (x86)/IIS/Microsoft Web Deploy V3/msdeploy.exe" -verb=sync -source:contentPath="D:\\try02" -dest:auto,computerName=https://CRLHS-PNMS07:8172/msdeploy.axd?site=TestSite,username="CONTOURSOFTWARE\\rehmayas",password="rehmayas1",authType="Basic" -enableRule:DoNotDeleteRule -enablerule:AppOffline -setParam:value="TestSite",kind=ProviderPath,scope=contentPath -AllowUntrusted="True" """
            
                println('Rollback - Prod - Dev');
            }
        }
    }

}     

