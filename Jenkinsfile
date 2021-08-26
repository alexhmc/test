node {
  def remote = [:]
  remote.name = 'ubuntu_server'
  remote.host = '192.168.186.134'
  remote.user = 'amejia'
  remote.password = 'warning93'
  remote.allowAnyHosts = true
  stage('GIT') {
    steps {
      checkout scm
    }
  }
  stage('Remote SSH') {
    sshCommand remote: remote, command:  "hostname"
  }
}
