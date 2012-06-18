Vocabulary Template
===================

This is the base repo for OData vocabulary definitions. It comes with a a recommended vocabulary spec template and some recommendations about publishing.

Fork this repo to create a vocabulary definition. If you do so, then GitHub will make it easy to see all the OData vocabularies that people are working on. Each will appear as a fork of this base template.

Directory Structure
-------------------

We recommend that you organize your vocabulary repository with the following structure. This will make it easy to work on your vocabulary, to publish it, and to keep a record of its history.

* Versions
  * VocabName.1.0.md
  * VocabName.1.1.md
  * ...
* VocabName.Current.md
* Vocabname.Next.md
* License.txt
* Readme.md
* Contrib.txt

Each version of the vocabulary is defined in a single specification file. In the above structure, these are the VocabName.*.md files. The file name for each of these includes the version to which it applies. There are two special versions.

VocabName.Current.md is always the same as the highest-numbered Versions/VocabName.x.y.md. This gives a URI that always represents the most recent fully released version of the vocabulary. That way people can choose to refer either to a particular version or to "the most recent version."

VocabName.Next.md is the file to work in. It always represents the next version of the vocabulary. This is the current best-known draft. It is not yet agreed upon. This should not be used as a vocabulary reference. However, it provides a place to work on extending the vocabulary.

Method of Work
--------------

We work entirely in VocabName.Next.md. We can use other supporting documents (such as the wiki for this repo) as supporting docs. However, the markdown file is the current proposal for the next version. This always represents our latest thinking.

From time to time VocabName.Next.md will reach a point that we decide is worth releasing. At that point, we delete VocabName.Current.md. We copy VocabName.Next.md to both current and to a correctly version-labeled file in the Versions directory. That is the official signal of a release: a new version appears in the Versions directory and VocabName.Current.md is updated.

Getting Started
---------------

There are a couple of things that you should do when you first start defining a vocabulary. Some of them are obvious; some are less so.

1. Fork this repo.
2. Rename VocabName.Next.md to match the name for your vocabulary (e.g., Display.Next.md).
3. Pick a license. This template includes a default option. This will work for many cases. But certain vocabulary-defining entities (such as standards organizations) will want to use other licenses. If you are using these licenses, update the CLA agreement to use the correct name for your vocabulary specification.
4. Fill in contributors.txt with any initial authors. Make sure you've got contributor license agreements from each author that will allow publishing under the above license.
5. Start writing your vocabulary. VocabName.Next.md includes a template structure that can get you started. You can vary from the structure, but this is a good starting point.
