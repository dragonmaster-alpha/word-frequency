# word_frequencies_api
Returns the most frequent words in a text file

# How to Run
1. Clone repo
2. Run; "npm install"
3. Run; "npm start"

# Example request

Input: Given N = 3 and a text file with the following contents:

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer id purus imperdiet, condimentum enim a, volutpat nisi. Donec ut egestas tellus, sed dignissim lorem. Phasellus tristique ex eu mollis rutrum. Sed interdum eget sapien in placerat. Quisque eu neque euismod, scelerisque mauris at, bibendum tellus. Pellentesque non sem nec dui feugiat posuere. Vivamus ac diam auctor, commodo enim sed, lobortis magna. Nullam nunc risus, hendrerit sed augue ac, imperdiet facilisis libero. Quisque non mollis purus. Nullam vitae ornare lectus, at pellentesque justo. Duis ultrices sem in mi luctus finibus. Ut id ligula ante.

Donec sit amet lacus turpis. Praesent vitae erat ac elit scelerisque faucibus nec sed dui. Suspendisse in imperdiet sapien. Donec efficitur ex lorem, a faucibus urna luctus sit amet. Pellentesque elementum euismod lorem, ac vulputate mauris iaculis quis. Ut in dolor sit amet leo ornare sagittis. Aliquam tincidunt mi vel lacus sodales, in placerat lorem gravida. Maecenas blandit mi auctor fringilla venenatis.

Sed eros justo, tincidunt non ornare at, auctor ut urna. Aliquam pharetra pulvinar sodales. Sed id purus id metus dapibus dignissim quis accumsan eros. Vestibulum et felis quis ex molestie condimentum. Proin ut diam feugiat, elementum felis sit amet, vulputate erat. Nullam quis cursus diam. Sed sit amet feugiat nulla, at semper orci. Suspendisse quis viverra magna. Donec eu tempor lacus. Suspendisse potenti. Quisque a magna non libero finibus accumsan imperdiet eget augue. Nulla elementum vestibulum dolor, ac porttitor dolor congue et. Aliquam cursus tempor erat vel vestibulum.

Quisque tempus velit ac congue porta. Proin sagittis tellus id gravida condimentum. Duis eu efficitur magna. Proin molestie tristique ex, quis rhoncus magna ornare ac. Curabitur et felis id enim pharetra pretium. Integer quis quam sodales, maximus magna id, porttitor mi. Nullam viverra magna sem, ut laoreet dolor mollis sit amet.

Phasellus vel dolor nibh. Nam ut efficitur quam, sed mattis turpis. Curabitur congue id mauris ut vulputate. Donec malesuada lectus at lorem blandit, nec facilisis mauris tincidunt. Suspendisse eget nibh eget elit sodales ullamcorper vitae a nunc. Morbi blandit viverra erat, sit amet fringilla lorem pellentesque id. Etiam sapien nulla, imperdiet vel sem vel, dignissim dapibus nisi. Aliquam erat volutpat. Duis bibendum nisl vitae tristique luctus. Nunc fringilla orci at urna sodales feugiat. Nam id diam auctor est mollis tempor at vitae risus. Nulla posuere mattis nibh, in viverra risus facilisis et. Suspendisse sed posuere mi, sed dictum sem. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Curabitur tristique ex vitae metus ornare, nec feugiat nunc rutrum. Donec commodo vehicula odio, sed faucibus ex tincidunt et.


Output: we expect the API to return the following JSON response: 

{
    "frequencies": [
        {
            "word": "sed",
            "count": 12
        },
        {
            "word": "id",
            "count": 10
        },
        {
            "word": "sit",
            "count": 8
        }
    ]
}

# IMPROVEMENTS WE COULDN'T IMPLEMENT
1. UNIT TEST: We ran out of time before we could complete the unit test, but all the other parts of the API works fine AND all other requirements have been met
2. We can upgrade APIs using TrieNode information. It's convenient for finding prefixes, counting numbers, and so forth.
The best references are all using TrieNode and in my experience, it's the fast way to find strings in large amount of data.
https://www.geeksforgeeks.org/find-the-k-most-frequent-words-from-a-file/
https://gist.github.com/tpae/72e1c54471e88b689f85ad2b3940a8f0
