simpleBuild {
 
    env = [
        FOO : 42,
        BAR : "YASS"
    ]
    
 

    before_script = "echo before"
    script = 'echo after $FOO'
    
    notifications = [
        email : "mneale@cloudbees.com"    
    ]
    stage('slack notification') {
               slackSend channel: 'rivet-jenkins', color: 'red', iconEmoji: '', message: 'Welcome to Jenkins slack', teamDomain: 'kaay', tokenCredentialId: 'Jenkins-slack', username: ''  
                }
    
}
