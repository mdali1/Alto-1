stage ( "unit test") {
   sh "pwd"
   echo "we are in unit test **** *** ** *"

node {
   git "https://github.com/forpix/Alto-1.git"
   sh "echo unit test app"
   echo 'we are inside the node block '
   echo" ====================================="
}

   stage ("test on supported OSes") {

parallel (
  windows: { node {
    sh "echo building on windows now"

 }},
  mac: { node {
    sh "echo building on mac now"
  }})
   
   }
