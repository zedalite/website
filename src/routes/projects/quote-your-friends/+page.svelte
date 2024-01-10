<script lang="ts">
  import type { PageData } from "./$types";
  import screenshot from "$lib/assets/app_example.jpg";

  export let data: PageData;
</script>

<div class="container mx-auto flex flex-col items-center gap-8 p-8">
  <h1 class="h1">
    <span class="bg-gradient-to-br from-blue-500 to-cyan-300 bg-clip-text text-transparent box-decoration-clone">
      Quote Your Friends App
    </span>
  </h1>
  <div class="flex gap-2">
    <a href="/projects" class="btn variant-ghost">
      <span class="material-symbols-outlined"> keyboard_backspace </span>
      <span>Browse</span>
    </a>
    <a href="https://quotes.zedalite.de/" target="_blank" rel="noreferrer noopener" class="btn variant-ghost">
      <span>Launch</span>
      <span class="material-symbols-outlined"> rocket_launch </span>
    </a>
  </div>
  <div class="flex gap-8">
    <img class="max-w-xs rounded-lg" src={screenshot} alt="App screenshot" />
    <div>
      <h3 class="h3 text-center">Welcome to QuoteYourFriends</h3>
      <h4 class="h4 text-center">the ultimate app for sharing and savoring meaningful moments through quotes!</h4>
      <br/>
      <p>
        Unlock the power of inspiration and connection with our innovative app that lets you effortlessly share your
        favorite quotes with friends and loved ones. With QuoteYourFriends, the art of sharing wisdom, humor, and
        profound thoughts has never been more delightful.
      </p>
      <ul class="list">
        <li>
          <p>
            <strong>Seamless Sharing</strong>
            : Share your favorite quotes with a simple tap. Whether it's a quote that resonates with
            you, brings a smile to your face, or ignites a spark of motivation, QuoteYourFriends makes sharing
            effortless and enjoyable.
          </p>
        </li>
        <li>
          <p>
            <strong>Instant Notifications</strong>
            : Stay connected with your friends in real-time! Receive instant notifications whenever a
            friend posts a new quote. Never miss a moment of inspiration and keep the conversation alive.
          </p>
        </li>
        <li>
          <p>
            <strong>Interactive Feed</strong>
            : Immerse yourself in a dynamic and engaging feed filled with quotes from your friends.
            Like, comment, and interact with the quotes that touch your heart or spark a conversation. QuoteYourFriends
            transforms sharing into a collaborative and communal experience.
          </p>
        </li>
        <li>
          <p>
            <strong>Personalized Profiles</strong>
            : Create your unique profile to showcase your favorite quotes, thoughts, and
            expressions. Let others get to know you through the words that resonate with your soul.
          </p>
        </li>
        <li>
          <p>
            <strong>Customizable Settings</strong>
            : Tailor your experience to suit your preferences. Choose notification settings,
            customize your feed, and make QuoteYourFriends uniquely yours.
          </p>
        </li>
      </ul>
    </div>
  </div>

  <a href="/projects/quote-your-friends/privacy-policy" class="btn variant-ghost">Privacy Policy</a>
</div>
