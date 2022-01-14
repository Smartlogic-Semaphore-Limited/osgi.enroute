@Library('smartlogic-common@v2') _

smartlogic([
  docker: "maven:3.8.3-jdk-8",
  builder: smartlogic.mavenBuilder(),
  archive: { archive() }
   ])

def archive() {
  if (!params.skipTests) {
    archiveArtifacts('**/*.log')
  }
}