# Hello, World!

Let's begin by exploring the Vala language and how we can start building stuff.

Create a directory to store our project files, let's create a file called `hello.vala` and inside it we include:

```cs
int main (string[] args) {
    stdout.printf ("Hello, World!\n");
    return 0;
}
```

The first thing to realize is that Vala requires a `main` entry point to start executing from, if you are coming from C this will be very familiar.

To run this, we use the `valac` (**Vala** **C**ompiler) command:

```sh
valac hello.vala
```

And now we can execute it:

```sh
./hello
```

This should print out `Hello, World!` as expected.

Behind the scenes Vala compiles down to C and then gets passed on to a C compiler, if we want we can easily inspect the generated C code by telling the Vala compiler to give us the generated C code:

```sh
valac -C hello.vala
```

The result is a `hello.c` file that we can see what Vala has generated for us.

Because of this, Vala is built around C and often interacts with C code so having a good foundation of programming in C can be helpful in easing the learning curve, but nonetheless Vala is a much higher level language thanks to GLib's constructs, so it should still be managable without any experience in C.

Congratulations! You've had your first taste of Vala, in the next lesson we will start getting serious and get a GTK application up and running.
