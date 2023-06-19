# Tips for updating website

## Prerequisite on MacOS

Following the instructions from [here](https://gist.github.com/MichaelCurrin/61053a564bdb3098bae11f949bab3578) (Step 1-3) 
and then the main README (Local Setup Standard).

## CV

- Path: pdf file goes to `assets/pdf`
- Page: configure the pdf name into `_pages/cv.md`

## Publications

Put the Bibtex entry into `_bibliography/papers.bib`, and then add the following elements to the Bibtex entry when applicable.

### html
You can add a line like `html="[URL]",` to the entry, where `[URL]` is the online version of your paper from the publisher.

**Need a comma before a new line**

### pdf
1. Put PDF file under `assets/pdf/[PDF_NAME].pdf`.
2. Add a line like `pdf="[PDF_NAME].pdf",` to the Bibtex entry


### Abstract
Add a line like `abstract="{ABSTRACT_TEXT}",` to the Bibtex entry

### Media coverage
1. Create a markdown file under `_news`, name it as `[PAPER_IDENTIFIER].md`
2. You can copy from a template [here](_news/whitney2017we.md), 
and then change title, date and context accordingly.
3. **Do not put `:` in the title. I am using `-` as a replacement**
4. Add URLs to the content in the format of `[TEXT](URL)`.
5. Add a line `media="[PAPER_IDENTIFIER]/index.html",` to the Bibtex entry (no `.md` in the `PAPER_IDENTIFIER`).


### Example

An example Bibtex entry looks like this

```
@article{liu2021engaging,
  title={Engaging teachers measuring the impact of teachers on student attendance in secondary school},
  author={Liu, Jing and Loeb, Susanna},
  abbr={JHR},
  journal={Journal of Human Resources},
  volume={56},
  number={2},
  pages={343--379},
  year={2021},
  publisher={University of Wisconsin Press},
  pdf="JHR_2021.pdf",
  media="liu2021engaging/index.html",
  html="http://jhr.uwpress.org/content/56/2/343.short",
  abstract="On average, secondary school students in the United States are absent from school three weeks per year. For this study, we are able to link middle and high school teachers to the class-attendance of students in their classrooms and create measures of teachers’ contributions to student class-attendance. We find systematic variation in teacher effectiveness at reducing unexcused class absences. These differences across teachers are as stable as those for student achievement, but teacher effectiveness on attendance only weakly correlates with their effects on achievement. A high value-added to attendance teacher has a stronger impact on students’ likelihood of finishing high school than does a high value-added to achievement teacher. Moreover, high value-added to attendance teachers can motivate students to pursue higher academic goals. These positive effects are particularly salient for low-achieving and low-attendance students."
}
```


# News / Announcements
- Turn it on `_pages/about.md`, news.
- Where to write: `_news`.