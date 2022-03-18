# beam-go
## Steps to run the beam-go
#### Download and Install
* Download and Install GO from [https://go.dev/doc/install](https://go.dev/doc/install)
#### Check Version
* After Downloading and Installing, Check your GO version using the command  `go version`
#### Create a project and a Repository
* Create a project with name beam-go in your 44-517 folder.
* Create a git repo with exactly the same name of your project in local machine i.e., beam-go.
* In your folder, run `go mod init github.com/vivekd31/beam-go`
#### Get the SDK and the examples
* command `go get -u github.com/apache/beam/sdks/v2/go/pkg/beam`
#### Add the input file
* create the sample.txt file and add content from Shakespeare sonnets.
#### Run WordCount
- To get wordcount.go run the command `go install github.com/apache/beam/sdks/v2/go/examples/wordcount`
- If you get an error like "missing go.sum entry for module providing package" then run the command ` go get github.com/apache/beam/sdks/v2/go/pkg/beam/io/filesystem/gcs@v2.37.0`
- To run the wordcount.go use the command `go run wordcount.go --input sample.txt --output vivekd31_counts`
- The output counts file will be generated in the project folder.
