---
layout: default
---

<style>
  /* Logo styles */
  .logo-container {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 30px;
  }
  
  .vlrb-logo {
    width: 160px;
    height: 160px;
    margin-bottom: 10px;
  }
  
  .hero {
    text-align: center;
    padding: 60px 20px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    border-radius: 10px;
    margin-bottom: 40px;
  }
  
  .hero h1 {
    font-size: 3em;
    margin-bottom: 20px;
    font-weight: bold;
  }
  
  .hero .tagline {
    font-size: 1.5em;
    margin-bottom: 30px;
    opacity: 0.9;
  }
  
  .hero .subtitle {
    font-size: 1.1em;
    margin-bottom: 40px;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.6;
  }
  
  .cta-button {
    display: inline-block;
    background: #000;
    color: white;
    padding: 15px 40px;
    border-radius: 50px;
    text-decoration: none;
    font-weight: bold;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    color: white;
  }
  
  .features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
    margin: 50px 0;
  }
  
  .feature {
    text-align: center;
    padding: 30px;
    background: #f8f9fa;
    border-radius: 10px;
    transition: transform 0.2s;
  }
  
  .feature:hover {
    transform: translateY(-5px);
  }
  
  .feature h3 {
    color: #667eea;
    margin-bottom: 15px;
  }
  
  .pricing {
    margin: 60px 0;
  }
  
  .pricing h2 {
    text-align: center;
    margin-bottom: 20px;
    font-size: 2.5em;
  }
  
  .pricing-toggle {
    text-align: center;
    margin-bottom: 40px;
  }
  
  .toggle-container {
    display: inline-flex;
    align-items: center;
    background: #f0f0f0;
    border-radius: 30px;
    padding: 5px;
  }
  
  .toggle-option {
    padding: 10px 20px;
    border-radius: 25px;
    cursor: pointer;
    transition: all 0.3s;
    font-weight: 500;
  }
  
  .toggle-option.active {
    background: #667eea;
    color: white;
  }
  
  .toggle-option .discount {
    font-size: 0.8em;
    margin-left: 5px;
    color: #28a745;
  }
  
  .toggle-option.active .discount {
    color: #90ee90;
  }
  
  .pricing-tiers {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
    max-width: 900px;
    margin: 0 auto;
  }
  
  .tier {
    background: white;
    border: 2px solid #eee;
    border-radius: 10px;
    padding: 30px;
    text-align: center;
    transition: all 0.3s;
    position: relative;
  }
  
  .tier.featured {
    border-color: #667eea;
    transform: scale(1.05);
  }
  
  .tier:hover {
    box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  }
  
  .tier h3 {
    color: #667eea;
    font-size: 1.8em;
    margin-bottom: 10px;
  }
  
  .price {
    font-size: 2.5em;
    font-weight: bold;
    margin: 20px 0 10px 0;
  }
  
  .price .period {
    font-size: 0.5em;
    color: #666;
  }
  
  .price-annual {
    display: none;
  }
  
  .savings-badge {
    background: #28a745;
    color: white;
    padding: 5px 15px;
    border-radius: 20px;
    font-size: 0.8em;
    margin: 10px 0;
    display: inline-block;
  }
  
  .tier ul {
    list-style: none;
    padding: 0;
    margin: 20px 0;
    text-align: left;
  }
  
  .tier li {
    padding: 8px 0;
    border-bottom: 1px solid #eee;
  }
  
  .tier li:before {
    content: "✓ ";
    color: #667eea;
    font-weight: bold;
  }
  
  .faq {
    max-width: 800px;
    margin: 60px auto;
  }
  
  .faq h2 {
    text-align: center;
    margin-bottom: 40px;
    font-size: 2.5em;
  }
  
  .faq-item {
    margin-bottom: 25px;
    padding: 20px;
    background: #f8f9fa;
    border-radius: 10px;
  }
  
  .faq-item h4 {
    color: #667eea;
    margin-bottom: 10px;
  }
  
  @media (max-width: 768px) {
    .hero h1 {
      font-size: 2em;
    }
    
    .hero .tagline {
      font-size: 1.2em;
    }
    
    .features {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="hero">
  <div class="logo-container">
    <img src="https://weberswords.github.io/vlrb/assets/images/vlrb-logo-dark.svg" alt="vlrb logo" class="vlrb-logo">
  </div>
  <h1>vlrb</h1>
  <p class="tagline">Stories beyond words</p>
  <p class="subtitle">For less than your daily coffee, vlrb lets you tell stories that text messages can't capture. Share authentic video moments with friends and build meaningful connections through visual storytelling.</p>
  <a href="{{ site.app_store_url }}" class="cta-button">Download on App Store</a>
</div>

<div class="features">
  <div class="feature">
    <h3>📱 No Storage Worries</h3>
    <p>Videos don't take up space on your phone unless you want them to. Keep your device clutter-free while sharing unlimited moments.</p>
  </div>
  
  <div class="feature">
    <h3>🎥 Longer Videos</h3>
    <p>Share more than iMessage allows. Express yourself fully with videos up to 10 minutes long in our premium tiers.</p>
  </div>
  
  <div class="feature">
    <h3>✨ Authentic Connection</h3>
    <p>Why type paragraphs when you can share a genuine moment? Tell your story with all the emotion and nuance that only video can deliver.</p>
  </div>
  
  <div class="feature">
    <h3>🔒 Private & Secure</h3>
    <p>Your moments are yours. End-to-end encryption ensures only you and your chosen recipients can view your vlrbs.</p>
  </div>
</div>

<div class="pricing">
  <h2>Simple, Transparent Pricing</h2>
  
  <div class="pricing-toggle">
    <div class="toggle-container">
      <div class="toggle-option active" onclick="togglePricing('monthly')">
        Monthly
      </div>
      <div class="toggle-option" onclick="togglePricing('annual')">
        Annual <span class="discount">Save 17%</span>
      </div>
    </div>
  </div>
  
  <div class="pricing-tiers">
    <div class="tier">
      <h3>Free</h3>
      <div class="price price-monthly">$0<span class="period">/forever</span></div>
      <div class="price price-annual" style="display: none;">$0<span class="period">/forever</span></div>
      <ul>
        <li>Share video moments up to 2 minutes</li>
        <li>Build meaningful connections</li>
        <li>Clean, ad-free interface</li>
        <li>Cloud storage for your vlrbs</li>
      </ul>
    </div>
    
    <div class="tier featured">
      <h3>Social</h3>
      <div class="price price-monthly">$4.99<span class="period">/month</span></div>
      <div class="price price-annual" style="display: none;">
        $49.99<span class="period">/year</span>
      </div>
      <div class="savings-badge price-annual" style="display: none;">Save $10/year</div>
      <ul>
        <li>Everything in Free</li>
        <li>Videos up to 10 minutes</li>
        <li>"Live Now" notifications</li>
        <li>3 "One more minute" extensions/week</li>
        <li>Priority delivery</li>
      </ul>
    </div>
    
    <div class="tier">
      <h3>Creator</h3>
      <div class="price price-monthly">$9.99<span class="period">/month</span></div>
      <div class="price price-annual" style="display: none;">
        $99.99<span class="period">/year</span>
      </div>
      <div class="savings-badge price-annual" style="display: none;">Save $20/year</div>
      <ul>
        <li>Everything in Social</li>
        <li>Unlimited "One more minute" extensions</li>
        <li>Custom expiration controls</li>
        <li>Picture-in-Picture support</li>
        <li>Priority support</li>
        <li>Advanced analytics</li>
      </ul>
    </div>
  </div>
</div>

<div class="faq">
  <h2>Frequently Asked Questions</h2>
  
  <div class="faq-item">
    <h4>How is vlrb different from Marco Polo or Loom?</h4>
    <p>vlrb focuses on authentic, ephemeral moments that don't clutter your phone. Unlike competitors, we prioritize storage efficiency and longer video capabilities while maintaining the spontaneous feel of genuine connection.</p>
  </div>
  
  <div class="faq-item">
    <h4>Do videos really not take up space?</h4>
    <p>Videos are stored in the cloud by default and only downloaded when you choose to save them. This keeps your phone storage free while letting you share as many moments as you want.</p>
  </div>
  
  <div class="faq-item">
    <h4>What happens when videos expire?</h4>
    <p>Expired videos are automatically removed from our servers. With our Creator tier, you can customize expiration times or keep videos indefinitely.</p>
  </div>
  
  <div class="faq-item">
    <h4>Is my content private and secure?</h4>
    <p>Absolutely. All videos are encrypted in transit and at rest. Only you and your intended recipients can view your content. We never access or analyze your videos.</p>
  </div>
</div>

<script>
function togglePricing(type) {
  const monthlyElements = document.querySelectorAll('.price-monthly');
  const annualElements = document.querySelectorAll('.price-annual');
  const toggleOptions = document.querySelectorAll('.toggle-option');
  
  if (type === 'monthly') {
    monthlyElements.forEach(el => el.style.display = 'block');
    annualElements.forEach(el => el.style.display = 'none');
    toggleOptions[0].classList.add('active');
    toggleOptions[1].classList.remove('active');
  } else {
    monthlyElements.forEach(el => el.style.display = 'none');
    annualElements.forEach(el => el.style.display = 'block');
    toggleOptions[0].classList.remove('active');
    toggleOptions[1].classList.add('active');
  }
}
</script>