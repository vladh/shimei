![shimei](images/shigoto_zaitaku_cat_woman.png)

# shimei

shimei is a super simple task management system. It is file-based and is meant to be used together with vim. However,
the ideas and simplicity are what's important, so you can customise this system to work with other technology (send a
PR!).

## Concepts

shimei relies on a few simple concepts.

* Projects have four-letter codes and look like this: `[proj]`. They mean what you would expect, different projects you
    work on.
* Goals also have four-letter codes, and are part of a project, so therefore look like this: `[proj!goal]`. Goals are
    very high-level objectives that potentially take a very long time to be completed. They should reflect your
    long-term objectives and values. The main point of goals is to make sure that the things you do day-to-day
    contribute towards you meeting some kind of goal.
* Tasks are individual items that need to be completed, and they belong to a project.

## Files

shimei reads files from the `~/.shimei` directory. The default setup has two files.


### `~/.shimei/todo.shimei`

The idea of the todo file is to list everything that needs to be done. It looks something like this:

```
[read]
    ! [intl] Read more books by authors from non-English-speaking countries
    - Read “Invisible Cities” by Italo Calvino
    - Read “The History of Western Philosophy” by Bertrand Russell

[song]
    ! [flut] Learn to play the flute
    - Play “The Gnostic Preludes” by John Zorn on flute
    - Find a place to take flute lessons
```

For each project, you can define the things that you want to do, and the goals for each project. When you finish a task,
delete it. Make sure to check on each goal periodically — they'll be highlighted in vim.

### `~/.shimei/log.shimei`

The idea of the log file is to write down everything you do each day. It looks something like this:

```
21-01-2022

    - [read!intl] Read a little bit of Invisible Cities

20-01-2022

    - [read] Read a bit of Pride and Prejudice
    - [song!flut] Learn how to play some major scales on the flute.
    - Plant some flowers in the garden
    - Play Minecraft

19-01-2022
    - Nothing! (and that's cool too)
```

Note that things you do on a particular day can correspond to a goal, a project, a task, or none of the above. The idea
is to make sure that on most days, you're doing something to advance one of your goals.

Note that a log item does not have to correspond to a task at all. Because tasks (the ones from the todo file) can often
represent more than can be done in one day, you can think of log items as potentially chipping away at a certain task.
It's nice to log cool things that you did on a certain day even if they have nothing to do with a task, goal, or
project. The things we do on any given day are often not pre-planned or “productive”, but those spontaneous
“unproductive” things often end up being super valuable to us anyway.

Everything is written in the imperative mood (e.g. “write...”, “play...”) so that you can just as easily write log
entries for future days, which can serve as your plan for the future.

## Credits

Icon by [irasutoya](https://www.irasutoya.com)
