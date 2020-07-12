- Plain Text / SSML - Add below text 

  - I'm learning Polly using AWS and CLI with lexicon XML format. / <speak>I'm learning Polly using AWS and CLI with lexicon XML format.</speak>

- Engine: Standard
- Voice: Joanna, Female
- Upload lexicons XML file 

- aws --region=us-west-2 polly list-lexicons
- aws --region=us-west-2 polly list-lexicons | grep Name
- aws --region=us-west-2 polly put-lexicon --name myFirstLexiconPut --content file://polly/myFirstLexiconPut.xml
