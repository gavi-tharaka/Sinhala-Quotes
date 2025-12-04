🇱🇰 1000 Sinhala Quotes JSON
Welcome to the Sinhala Quotes JSON repository! This project provides a curated collection of over 1000 Sinhala quotes structured in a developer-friendly JSON format.
This dataset is perfect for building:
 * Quote of the Day applications
 * Social media bots
 * Sinhala language learning tools
 * Websites displaying random thoughts
📂 Data Structure
The data is stored in quotes.json as an array of objects. Each object contains a unique id and the quote string.
Format:
[
  {
    "id": 1,
    "quote": "ඔබට නවතින්නට සිතුන විට, ඔබ පටන් ගත්තේ ඇයි දැයි සිහිපත් කරන්න."
  },
  {
    "id": 2,
    "quote": "උත්සාහය දිනක දිනුම ගෙනෙයි."
  },
  {
    "id": 3,
    "quote": "ජයග්‍රහණය යනු වැටීම නොව, වැටුන සෑම විටම නැගී සිටීමයි."
  }
]

🚀 How to Use
1. Direct Download
Simply download the quotes.json file from this repository to use it locally.
2. Fetch via API (Raw GitHub URL)
You can fetch the data directly into your application using the raw content URL.
Endpoint:
https://raw.githubusercontent.com/gavi-tharaka/Sinhala-Quotes/main/quotes.json
JavaScript Example
Here is a simple example of how to fetch a random quote using JavaScript:
const url = '[https://raw.githubusercontent.com/gavi-tharaka/Sinhala-Quotes/main/quotes.json](https://raw.githubusercontent.com/gavi-tharaka/Sinhala-Quotes/main/quotes.json)';

fetch(url)
  .then(response => response.json())
  .then(data => {
    // Get a random quote
    const randomIndex = Math.floor(Math.random() * data.length);
    const randomQuote = data[randomIndex];
    
    console.log(`Quote ID: ${randomQuote.id}`);
    console.log(`Message: ${randomQuote.quote}`);
  })
  .catch(error => console.error('Error fetching quotes:', error));

🤝 Contributing
Contributions are welcome! If you have more inspirational Sinhala quotes to share:
 * Fork this repository.
 * Add your quotes to quotes.json (Please maintain the id order).
 * Commit your changes and open a Pull Request.
📝 License
This project is open source and available under the MIT License.
