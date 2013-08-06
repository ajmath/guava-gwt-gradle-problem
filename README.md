Basic example of problem mentioned in the following posts

http://stackoverflow.com/questions/17147234/gradle-guava-gwt-abstractiterator-class-duplicated

http://forums.gradle.org/gradle/topics/compilation_fails_when_i_use_guavas_optional_class_duplicate_class_com_google_common_collect_abstractiterator

http://stackoverflow.com/questions/17104455/guava-abstractiterator-duplicate-class


Adding
```
tasks.withType(JavaCompile) {
    options.compilerArgs << '-implicit:none'
}
```
does not help.

I've also added an example of a similar ant build.xml which does not have any problems compiling the code

