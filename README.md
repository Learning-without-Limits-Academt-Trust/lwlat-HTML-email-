# LwLAT Email Builder

A single web page for making bright, well-designed emails to send to colleagues from Outlook. You build the email from blocks, see it as it will look, then press **Copy for Outlook** and paste it into the body of a new message. Colleagues see the design in the email itself, not as an attachment.

It can also take an email designed in Canva and get it into Outlook in the same way.

Everything happens in your browser. Nothing is sent to a server and there is no account to sign in to.

## Making an email

The builder works like Mailchimp. The email sits in the middle of the screen and you edit it where it is.

1. Choose **Start from a template** on the left, or edit the email already there.
2. **Click any words in the email** and type to change them. In text blocks, select words to make them bold or italic, add a link or start a bullet list from the small black toolbar.
3. **Click a block** to see its settings on the left, such as colours, pictures, links and alignment.
4. **Add a block** by dragging it from the left into the email, or by clicking it to drop it under the block you have selected.
5. **Move or remove a block** with the buttons that appear beside it. The dotted handle lets you drag it to a new place.
6. Use the **Styles** tab for the colour theme, font, button shape and window bar.
7. Press **Preview** to see it on a desktop and on a phone.
8. Press **Copy for Outlook**. In Outlook, start a new email, click in the body and press **Ctrl+V**. Add the subject and recipients and send.

**Undo** and **Redo** are at the top, and work with Ctrl+Z and Ctrl+Y when you are not typing. To drop a picture straight in, drag a photo from your computer onto the email.

Always send the first copy to yourself, and open it in Outlook on a PC and on a phone, before sending it to colleagues.

## The look

The emails follow the Pulse homepage Concept C specification: a teal backdrop, white "app window" cards with red, orange and light-green window dots and a teal pill label, an orange announcement bar with dark text, and date cards coloured by type (trust events in darkest teal, deadlines in orange, meetings in purple). Small text is only ever set in darkest teal, grey or near-black. Light green is used for large headline words on dark backgrounds only.

The builder screen uses Source Sans 3 as a stand-in for The Sans. Emails use Arial or another web-safe font, because Outlook swaps any font it does not have for Times New Roman.

## Using a Canva email

1. In Canva, create a design using the **Email** design type.
2. Choose **Share**, then the HTML export option, and **Copy HTML**.
3. In the builder, choose **More**, then **Use a Canva email**, and paste it in.
4. Press **Copy for Outlook** and paste into a new email.

Use Canva text boxes for words. Text grouped with a picture is turned into an image, which cannot be read when Outlook blocks pictures or by a screen reader.

## Pictures

There are two ways to add a picture:

- **Link to a picture already online** (for example on the trust website). This is the most reliable option and keeps the email small.
- **Upload** from your computer. The picture is shrunk and built into the email. This works well in new Outlook and Outlook on the web. Check it with a test send in classic Outlook.

Always fill in the description. It is shown when pictures are blocked and read aloud by screen readers.

Only use photographs of learners where the school holds photo consent for internal use.

## Saving and sharing designs

Your current email is kept in your browser. Under **More**, **Save design file** downloads a small file you can open later with **Open design file**, or pass to a colleague to reuse as a template.

## How it is built, and why

| Choice | Reason |
| --- | --- |
| One HTML file, no server | Nothing to maintain, nothing to secure, free on Netlify |
| Layout made of tables with every style written inline | Classic Outlook for Windows draws emails with Microsoft Word, which ignores most modern web layout |
| Fixed 600px width | Looks the same in classic Outlook, new Outlook and Outlook on the web. Phones shrink it to fit |
| Web-safe fonts only (Arial, Verdana, Trebuchet, Georgia) | Outlook replaces other fonts with Times New Roman |
| Rounded corners on buttons and boxes | Show in new Outlook and on phones. Classic Outlook shows square corners, which still look fine |

## Putting it live on Netlify

1. In Netlify choose **Add new site**, then **Import an existing project**, and pick this repository.
2. Leave the build settings as they are. Netlify reads them from `netlify.toml`.
3. Deploy. The page is marked so search engines do not list it.

You can also simply open `index.html` from your computer. It works the same way.
