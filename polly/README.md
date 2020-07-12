- Plain Text / SSML - Add below text 

  - I'm learning Polly using AWS and CLI with lexicon XML format. / <speak>I'm learning Polly using AWS and CLI with lexicon XML format.</speak>

- Engine: Standard
- Voice: Joanna, Female
- Upload lexicons XML file 

- aws --region=us-west-2 polly list-lexicons
- aws --region=us-west-2 polly list-lexicons | grep Name
- aws --region=us-west-2 polly put-lexicon --name myFirstLexiconPut --content file://polly/myFirstLexiconPut.xml

- <speak>The more I <w role="amazon:VBD">read</w> last week, the more I want to <w role="amazon:VB">read</w></speak>
- <speak>Every day feels like <say-as interpret-as="date" format="dm">25/12</say-as>.</speak>
- <speak>It feels like I'm living in <say-as interpret-as="date" format="y">1980</say-as>.</speak>
- <speak>It feels like I'm living in <say-as interpret-as="date" format="y">1980</say-as>, but I feel <sub alias="great">gr8</sub></speak>
- <speak>It feels like I'm living in <say-as interpret-as="date" format="y">1980</say-as>, but I feel <prosody rate="slow" volume="x-loud"><sub alias="great">gr8</sub></prosody></speak>
