# Getting back into Go, trying to organize things

## Projects to study
### concurrent file search grep command
- to get familiar https://en.wikipedia.org/wiki/Grep

#### Main features of the grep command by ChatGPT
##### What are the main features of the grep command?
The grep command is a powerful tool used for searching and filtering text data in Unix-based operating systems. Some of the main features of the grep command include:

Search for patterns: The grep command searches for specific patterns in a file or output stream and prints out the lines that match those patterns. You can search for words, phrases, or patterns of characters within a file or output stream.

Regular expression support: grep supports the use of regular expressions for pattern matching. This allows for more advanced and flexible searches.

Case-insensitive search: You can use the -i option with grep to perform a case-insensitive search, meaning that the search will match both uppercase and lowercase letters.

Recursive search: With the -r or -R option, grep can search for a pattern recursively in all files and directories within a given directory.

Inverted search: You can use the -v option to perform an inverted search, which means that grep will print out all lines that do not match the pattern.

Line number display: You can use the -n option to print the line numbers of the matched lines.

Multiple file search: You can use the grep command to search for a pattern in multiple files by specifying the file names as command line arguments or using wildcards.

Pipe support: grep can be used in combination with other commands by piping the output of one command into grep as input.

### ChatGPT CLI
It would be cool to have ChatGPT integrated to my terminal, not to simply ask questions through the terminal but to get its answers as inputs. 
```
  gptcli Remove my current Go installation and install the latest one.

  # it proceeds to output the commands in order
  sudo rm -rf /usr/local/go;
  wget /path/to/latest/go/tar.gz;
  tar -C /usr/local -xzf go.X.X.tar.gz;
  export PATH=$PATH:/usr/local/go/bin
```
Obviously there could a million edge case scenarios.

#### Flag ideas
- -q to simply ask questions
- -cli to use the responses directly as commands
- -list to list chats
- -c [chat name] to keep asking questions into the same chat

## Some resources
- Simple references https://gobyexample.com/
- Deeper references https://go.dev/doc/effective_go
- "best practices"  https://github.com/betrybe/playbook-go/blob/main/README_EN.md
- Discord Bot https://github.com/bwmarrin/discordgo

#### DevOps stuff
- https://thechief.io/c/editorial/why-golang-is-widely-used-in-the-devops-and-cloud-native-space/
- What is a Kubernetes Operator? https://www.redhat.com/en/topics/containers/what-is-a-kubernetes-operator
- Operator pattern https://kubernetes.io/docs/concepts/extend-kubernetes/operator/
