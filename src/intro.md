# Introduction

This book is a comprehensive tutorial to get started in developing applications for the GNOME platform in Vala, making use of GTK4 and Adwaita.

We will dive deep into how projects are structured and make use of Meson as our build tool and include guides for Flatpaks as well in an attempt to make this tutorial as practical as possible for real world use.

Additonally, there will be a section for recipes, which will include examples to solve a specific problem which may come in handy on your journey later on.

## The GNOME Platform

This book will primarily target GNOME by using their style guidelines and the Adwaita library, but the general structure of the guide can still be helpful for creating generic GTK4 programs or using another platform like elementaryOS with their Granite library but it's up to the reader to replace the parts accordingly.

GNOME as a platform consists of many parts such as:

* **GLib**: Provides many general purpose utilities that is used throughout GNOME technologies.
* **GObject**: Object oriented library that many of GNOME's projects are built on.
* **GTK**: Widget toolkit library built on top of GLib and GObject
* **Adwaita**: Additional GNOME specific widgets and styling built on top of GTK.

You do not need to be using GNOME as your desktop, as long as you have the necessary libraries, applications built for GNOME will run on any Linux distribution and desktop environment and even on macOS and Windows!

## Why Vala?

Vala is a programming language also built by the GNOME team, its syntax is inspired by C# and is built to leverage GLib and GObject at its core, it also includes out of the box bindings for many libraries including all of the GNOME stack such as GTK.

Since GTK is built around GObject, using GTK bindings in another programming language also comes with its burden of having to correctly manage GObjects in said language which may not always feel idiomatic.

Since Vala is built exactly to leverage GObject and interoperate in this world, it makes an excellent choice to develop programs using GTK.

Even if you choose to use a different programming language in the future, the experience you will learn here will come in handy.
