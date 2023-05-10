# Lab Report 3: Researching Commands

---

## Chosen Command: grep

## Command Option 1: `-r`
```
[cs15lsp23if@ieng6-202]:technical:101$ grep -r "everyone" 911report
911report/chapter-1.txt:    UAL 175: Yeah. We figured we'd wait to go to your center. Ah, we heard a suspicious transmission on our departure out of Boston, ah, with someone, ah, it sounded like someone keyed the mikes and said ah everyone ah stay in your seats.
911report/chapter-1.txt:    When they learned a second plane had struck the World Trade Center, nearly everyone in the White House told us, they immediately knew it was not an accident. The Secret Service initiated a number of security enhancements around the White House complex. The officials who issued these orders did not know that there were additional hijacked aircraft, or that one such aircraft was en route to Washington. These measures were precautionary steps taken because of the strikes in New York.
911report/chapter-11.txt:                is that everyone had the job. The CIA's deputy director for operations, James
911report/chapter-11.txt:            Headquarters tended to support and facilitate, trying to make sure everyone was in
911report/chapter-11.txt:            Why was this so? Most obviously, it was because everyone was already on edge with the
911report/chapter-13.2.txt:                after takeoff,"like someone keyed the mike and said everyone stay in your seats."
911report/chapter-13.5.txt:                those that everyone assumes somebody else is taking care of. It includes
911report/chapter-3.txt:                the FBI field offices in the United States, everyone in the Directorate of
911report/chapter-3.txt:                last sighting of Bin Ladin and that this persuaded everyone that the chance of
911report/chapter-3.txt:                dangerous, and it played more to their skills and experience. But everyone knew that
911report/chapter-3.txt:                QAEDA'S INITIAL ASSAULTS 135 and do something that everyone would later regret.
911report/chapter-5.txt:                insisted that everyone he had selected receive the training.
911report/chapter-7.txt:                Although Khallad claims not to recall everyone from this group who was later chosen
911report/chapter-8.txt:                said, it could not "get any worse." Not everyone was
911report/chapter-8.txt:            It is now clear that everyone involved was confused about the rules governing the
911report/chapter-9.txt:                channel and repeated it to everyone they came across. The chief on the 23rd floor
```

```
[cs15lsp23if@ieng6-202]:technical:108$ grep -r "plant" 911report
911report/chapter-13.4.txt:                intended role as one of the five operatives who would plant bombs on board the
911report/chapter-13.5.txt:                targeting a nuclear power plant as part of his initial proposal for the planes
911report/chapter-13.5.txt:                operation. See chapter 5.2. He has also stated that Atta included a nuclear plant in
911report/chapter-2.txt:                transplant his whole organization to Sudan. Turabi headed the National Islamic Front
911report/chapter-3.txt:                Ramzi Yousef, the Sunni extremist who planted the bomb, said later that he had hoped
911report/chapter-3.txt:                to Bin Ladin. The other was al Shifa, a Khartoum pharmaceutical plant, which
911report/chapter-3.txt:                INITIAL ASSAULTS 117 that a soil sample from the vicinity of the al Shifa plant had
911report/chapter-3.txt:                plant in Sudan." Senior State Department officials
911report/chapter-5.txt:                headquarters, nuclear power plants, and the tallest buildings in California and the
911report/chapter-7.txt:                schemes, such as buying four tons of ammonium nitrate for bombs to be planted on
```

*Source: I found out about this grep option from [this article about grep commands]https://www.tutorialspoint.com/unix_commands/grep.htm*

## Command Option 2: `-l`
```
[cs15lsp23if@ieng6-202]:technical:104$ grep -l "everyone" 911report/*.txt
911report/chapter-1.txt
911report/chapter-11.txt
911report/chapter-13.2.txt
911report/chapter-13.5.txt
911report/chapter-3.txt
911report/chapter-5.txt
911report/chapter-7.txt
911report/chapter-8.txt
911report/chapter-9.txt
```

```
[cs15lsp23if@ieng6-202]:technical:105$ grep -l "fire" 911report/*.txt
911report/chapter-1.txt
911report/chapter-10.txt
911report/chapter-11.txt
911report/chapter-13.1.txt
911report/chapter-13.2.txt
911report/chapter-13.3.txt
911report/chapter-13.4.txt
911report/chapter-13.5.txt
911report/chapter-2.txt
911report/chapter-3.txt
911report/chapter-5.txt
911report/chapter-6.txt
911report/chapter-7.txt
911report/chapter-9.txt
```

## Command Option 3: `-L`
```
[cs15lsp23if@ieng6-202]:technical:110$ grep -L "everyone" 911report/*.txt
911report/chapter-10.txt
911report/chapter-12.txt
911report/chapter-13.1.txt
911report/chapter-13.3.txt
911report/chapter-13.4.txt
911report/chapter-2.txt
911report/chapter-6.txt
911report/preface.txt
```

```
[cs15lsp23if@ieng6-202]:technical:107$ grep -L "fire" 911report/*.txt
911report/chapter-12.txt
911report/chapter-8.txt
911report/preface.txt
```

## Command Option 4: `-c`
```
[cs15lsp23if@ieng6-202]:technical:109$ grep -c "everyone" 911report/*.txt
911report/chapter-1.txt:2
911report/chapter-10.txt:0
911report/chapter-11.txt:3
911report/chapter-12.txt:0
911report/chapter-13.1.txt:0
911report/chapter-13.2.txt:1
911report/chapter-13.3.txt:0
911report/chapter-13.4.txt:0
911report/chapter-13.5.txt:1
911report/chapter-2.txt:0
911report/chapter-3.txt:4
911report/chapter-5.txt:1
911report/chapter-6.txt:0
911report/chapter-7.txt:1
911report/chapter-8.txt:2
911report/chapter-9.txt:1
911report/preface.txt:0
```

```
[cs15lsp23if@ieng6-202]:technical:106$ grep -c "fire" 911report/*.txt
911report/chapter-1.txt:1
911report/chapter-10.txt:1
911report/chapter-11.txt:1
911report/chapter-12.txt:0
911report/chapter-13.1.txt:4
911report/chapter-13.2.txt:3
911report/chapter-13.3.txt:1
911report/chapter-13.4.txt:2
911report/chapter-13.5.txt:57
911report/chapter-2.txt:1
911report/chapter-3.txt:6
911report/chapter-5.txt:1
911report/chapter-6.txt:4
911report/chapter-7.txt:1
911report/chapter-8.txt:0
911report/chapter-9.txt:145
911report/preface.txt:0
```

