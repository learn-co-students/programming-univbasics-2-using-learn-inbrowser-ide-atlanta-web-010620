# Programming as Conversation 2: Using Learn In-Browser IDE

## Learning Goals

- Provide the command to run a file through Ruby
- Compare running a Ruby file versus using IRB
- Run a Ruby program in the Learn In-Browser IDE

## Introduction

Thus far, we have been using Ruby's IRB inside of the Learn In-Browser IDE.  As
a quick reminder, IDE stands for Integrated Development Environment: a set of
tools that lets you read, write, and run code.  In "Programming as Conversation
1" we were clicking in the small, black window at the bottom (the Terminal) and
were running IRB there. Here we'll start using the rest of the IDE.

When we were writing simple expressions, we could have a direct conversation
with Ruby in IRB. We didn't really need to save our work as a quick copy and
paste was sufficient to get our world loaded back up.

However, we're going to start writing longer programs now and we're going to be
quite cross if we find our program's code missing. In this lesson, we'll
demonstrate how to create and run a Ruby file.

## Before We Start

If you have not used the Learn In-Browser IDE while following along, to quickly
review: while viewing this lesson in Learn.co, in the upper-right section of the
screen, you should see a **Sandbox*** button:

![Sandbox button](https://curriculum-content.s3.amazonaws.com/prework/sandbox-learn.png)

Clicking this button will open the In-Browser IDE. If the **Sandbox** button is
not currently present, we ask that you do two things:

- In the upper-right section of the screen is a small gray button with a flag on
  it. Clicking this button will start the process of opening an issue on this
  lesson's GitHub repository. Please fill out the title and description and
  submit an issue. Opening an issue here will help identify problems that may be
  affecting multiple students.

  ![Issue flag button](https://curriculum-content.s3.amazonaws.com/prework/issue_flag_button.png)

- After creating an issue, click the Ask a Question button to connect with a
  coach that can give you further guidance on the next steps.

   ![Ask a Question button](https://curriculum-content.s3.amazonaws.com/prework/AAQ_button.png)

A lot of upcoming content will assume that you are able to access this IDE, so
now is a good time to make sure you are set up. For additional information on the IDE,
check out [this article][ide learn guide].

[ide learn guide]: https://help.learn.co/en/articles/1392337-ide-in-browser

If everything is working as it should, clicking the **Sandbox** button will open
the In-Browser IDE.

## Provide the Command to Run a File Through Ruby

To tell Ruby to "read and run" a file, we use the command:

`ruby name_of_file`

By convention, as Ruby developers, we like to put `.rb` at the end of a file
name. It's not required, but it's helpful to remind us that the contents are
meant for **R**u**B**y. Eventually, you might learn dozens of programming
languages, and it's helpful to have a little visual clue about which language
knows how to read the conversation recorded inside.

For example:

`ruby demo.rb`

would be a typical command.

## Compare Running a Ruby File Versus Using IRB

When you run `ruby name_of_file.rb`, it's the same as if you typed in all the
contents of `name_of_file` into IRB. Any `puts` calls will print things out,
any _expression_ will be evaluated, and any _statements_ will be processed
according to the rules of Ruby. Also, if anything goes wrong, Ruby will print
an error message which will tell you which line in the file had the problem.

Remember, Ruby is not your enemy. It's your conversational partner and if you
say something it doesn't understand, it does its best to tell you how to help it
along.

## Run a Ruby Program in the Learn In-Browser IDE

To practice running a file, you'll first _need a file to run_. Let's create
this file and run it in Learn's In-Browser IDE.

Open the IDE and click on the Terminal. In the Terminal, type:

```sh
touch example_file.rb
```

A file named `example_file.rb` will appear in the file navigation

![sandbox files](https://curriculum-content.s3.amazonaws.com/prework/in-browser-ide-file-nav.png)

Click `example_file.rb` to open the file in the editor

![file editor](https://curriculum-content.s3.amazonaws.com/prework/in-browser-ide-file-editor.png)

Anything Ruby code we write in here will get executed when the file is run.
Let's give this file something to do. In the file editor, write the following:

```rb
puts "Hello World"
```

When done, click on the Terminal and run the file:

```sh
ruby example_file.rb
```

The Terminal should print out `Hello World`. You've written a program!

**Note**: As an alternative to the previous instructions, you can also use the
In-Browser IDE's **Create New** button the create the file needed. Here's an
animation showing this method:

![Demo Animation](https://curriculum-content.s3.amazonaws.com/programming-univbasics-2/learn-ibide-create-run-ruby-file-sm.gif)

## ALTERNATIVE: Local Development

We've made this module runnable in the In-Browser IDE so that you don't have to
learn a lot about the CLI environment or install a lot of engineering tools to
get going. In time, we'll teach you to install these, of course. And once in a
Flatiron School cohort, you'll be using them all the time and will leave the
In-Browser IDE behind.

Right now, however, we want to make sure you're focused on "learning Ruby" not
"learning to set up a development environment."

If you're already familiar with the Terminal and command-line interface
environment and would prefer to follow the lessons on your local computer, feel
free to do so instead of using the Learn In-Browser IDE, just keep in mind that
these materials may assume you're using the In-Browser IDE.

## Conclusion

OK, OK, no more delays! You have your tools: `ruby`, the in-browser IDE. You
know what we're going to study: statements. No more prologue, no more
introductions. We're going to start off by working with statements.
