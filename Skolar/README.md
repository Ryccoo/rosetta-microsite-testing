Basic usage of liquid microsite system

Tags :
{% image_path [image name] %}
  - returns path to image, has two levels of search
    1. first search in family images folder
    2. if the file is not present at family images folder, looks up at common/images
    3. else return common/images/not-found.jpg

{% file_path [file name] %}
  - looks up a file name in family/files folder
  - returns path to file or empty string if file does not exist

{% buy_buton %}
  - finds family starting price and creates a buy button element with found price
  - create button with NA price if there are no prices for family

{% ask_us_now_form %}
  - create ask us form for family

{% font_tester %}
  - create font test area for family

{% web_performance %}
  - create web performace area for family

{% language_count_for [font name] %}
  - counts number of supported languages for font [font name]
  - returns "Language not found" if language is not present at database

{% designers_info %}
  - return area with involved designers

{% charsets_selector %}
  - create area with charset selection and download button

More info in site.luqid.html




File Structure :
  - microsite
    - common
      - images
        // images shared on multiple microsites
    - Skolar
      - images
        // images used on current family microsite
        - web performance
          // images for web perofrmance
      - files
        // files used on current family microsite
        - charsets
          // charsets for family
      - site.liquid.html
        // microsite html

