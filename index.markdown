---
layout: default
---

<style>
  /* CSS Custom Properties for easy theming */
  :root {
    --cream-bg: #F5F1E8;
    --warm-paper: #FFF8F0;
    --aged-paper: #F5E6D3;
    --leather-brown: #7A5F3A;
    --ink-blue: #2C3539;
    --dusty-rose: #D4978A;
    --dusty-rose-dark: #9E6358;
    --terracotta: #C87E70;
    --sage-green: #A8B5A0;
    --muted-teal: #8BA89F;
    --text-brown: #3A342F;
    --text-brown-light: #4A3F35;
    --border-tan: #E3DDD3;
    --border-warm: #D9D0C3;
  }

  /* Hero Section - Warm & Inviting */
  .hero {
    text-align: center;
    padding: 4rem 1.5rem;
    background: linear-gradient(145deg, var(--warm-paper) 0%, var(--aged-paper) 100%);
    border: 1px solid var(--border-tan);
    border-radius: 16px;
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background:
      radial-gradient(circle at 20% 80%, rgba(212, 151, 138, 0.08) 0%, transparent 50%),
      radial-gradient(circle at 80% 20%, rgba(168, 181, 160, 0.08) 0%, transparent 50%);
    pointer-events: none;
  }

  .hero > * {
    position: relative;
    z-index: 1;
  }

  .logo-container {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 1.5rem;
  }

  .vlrb-logo {
    width: 120px;
    height: 120px;
    filter: drop-shadow(0 4px 12px rgba(58, 52, 47, 0.1));
  }

  .hero h1 {
    font-size: 2.75rem;
    margin-bottom: 0.5rem;
    color: var(--text-brown);
    font-weight: 700;
    letter-spacing: -0.02em;
  }

  .hero .tagline {
    font-size: 1.35rem;
    margin-bottom: 1.5rem;
    color: var(--leather-brown);
    font-weight: 500;
    font-style: italic;
  }

  .hero .subtitle {
    font-size: 1.1rem;
    margin-bottom: 2rem;
    max-width: 560px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
    color: var(--text-brown-light);
  }

  .cta-button {
    display: inline-block;
    background: var(--leather-brown);
    color: var(--warm-paper);
    padding: 1rem 2rem;
    border-radius: 12px;
    text-decoration: none;
    font-weight: 600;
    font-size: 1rem;
    transition: all 0.25s ease;
    border: none;
    box-shadow: 0 4px 12px rgba(122, 95, 58, 0.2);
  }

  .cta-button:hover {
    background: #6A5232;
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(122, 95, 58, 0.25);
    color: var(--warm-paper);
  }

  .cta-button:active {
    transform: translateY(0);
  }

  /* Decorative Divider */
  .section-divider {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 3rem 0;
    gap: 1rem;
  }

  .section-divider::before,
  .section-divider::after {
    content: '';
    height: 1px;
    width: 60px;
    background: var(--border-tan);
  }

  .section-divider .icon {
    font-size: 1.25rem;
    color: var(--dusty-rose);
    opacity: 0.8;
  }

  /* Features Section */
  .features-section {
    margin: 3rem 0;
  }

  .section-title {
    text-align: center;
    font-size: 1.75rem;
    color: var(--text-brown);
    margin-bottom: 0.5rem;
    font-weight: 600;
  }

  .section-subtitle {
    text-align: center;
    color: var(--text-brown-light);
    margin-bottom: 2.5rem;
    font-size: 1.05rem;
  }

  .features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 1.5rem;
  }

  .feature {
    background: var(--warm-paper);
    border: 1px solid var(--border-tan);
    border-radius: 12px;
    padding: 1.75rem;
    transition: all 0.25s ease;
  }

  .feature:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 24px rgba(58, 52, 47, 0.08);
    border-color: var(--border-warm);
  }

  .feature-icon {
    width: 48px;
    height: 48px;
    background: linear-gradient(135deg, var(--aged-paper) 0%, var(--border-tan) 100%);
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 1rem;
    font-size: 1.5rem;
  }

  .feature h3 {
    color: var(--leather-brown);
    margin-bottom: 0.75rem;
    font-size: 1.15rem;
    font-weight: 600;
  }

  .feature p {
    color: var(--text-brown-light);
    font-size: 0.95rem;
    line-height: 1.6;
    margin: 0;
  }

  /* Pricing Section */
  .pricing {
    margin: 4rem 0;
    padding: 3rem 0;
  }

  .pricing-intro {
    text-align: center;
    max-width: 540px;
    margin: 0 auto 2.5rem;
    color: var(--text-brown-light);
    line-height: 1.7;
  }

  .pricing-tiers {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.5rem;
    max-width: 960px;
    margin: 0 auto;
  }

  .tier {
    background: var(--warm-paper);
    border: 1px solid var(--border-tan);
    border-radius: 16px;
    padding: 2rem;
    text-align: center;
    transition: all 0.25s ease;
    position: relative;
  }

  .tier:hover {
    box-shadow: 0 8px 32px rgba(58, 52, 47, 0.1);
  }

  .tier.featured {
    border: 2px solid var(--dusty-rose);
    background: linear-gradient(to bottom, var(--warm-paper) 0%, rgba(212, 151, 138, 0.05) 100%);
  }

  .tier.featured::before {
    content: 'Most Popular';
    position: absolute;
    top: -12px;
    left: 50%;
    transform: translateX(-50%);
    background: var(--dusty-rose-dark);
    color: var(--warm-paper);
    font-size: 0.75rem;
    font-weight: 600;
    padding: 0.35rem 1rem;
    border-radius: 20px;
    letter-spacing: 0.02em;
  }

  .tier-icon {
    font-size: 2rem;
    margin-bottom: 0.75rem;
  }

  .tier h3 {
    color: var(--leather-brown);
    font-size: 1.35rem;
    margin-bottom: 0.5rem;
    font-weight: 600;
  }

  .tier .price {
    font-size: 2rem;
    font-weight: 700;
    color: var(--text-brown);
    margin: 1rem 0 0.25rem;
  }

  .tier .price .period {
    font-size: 0.9rem;
    font-weight: 400;
    color: var(--text-brown-light);
  }

  .tier .price-note {
    font-size: 0.85rem;
    color: var(--text-brown-light);
    margin-bottom: 1.25rem;
  }

  .tier ul {
    list-style: none;
    padding: 0;
    margin: 1.5rem 0;
    text-align: left;
  }

  .tier li {
    padding: 0.6rem 0;
    border-bottom: 1px solid var(--border-tan);
    color: var(--text-brown-light);
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    gap: 0.6rem;
  }

  .tier li:last-child {
    border-bottom: none;
  }

  .tier li::before {
    content: "~";
    color: var(--sage-green);
    font-weight: 600;
    flex-shrink: 0;
    margin-top: 0.05rem;
  }

  /* FAQ Section */
  .faq {
    max-width: 720px;
    margin: 4rem auto;
    padding: 0 1rem;
  }

  .faq-item {
    margin-bottom: 1.25rem;
    background: var(--warm-paper);
    border: 1px solid var(--border-tan);
    border-radius: 12px;
    padding: 1.5rem;
    transition: all 0.2s ease;
  }

  .faq-item:hover {
    border-color: var(--border-warm);
  }

  .faq-item h4 {
    color: var(--leather-brown);
    margin-bottom: 0.75rem;
    font-size: 1.05rem;
    font-weight: 600;
    line-height: 1.4;
  }

  .faq-item p {
    color: var(--text-brown-light);
    font-size: 0.95rem;
    line-height: 1.65;
    margin: 0;
  }

  /* Closing Section */
  .closing {
    text-align: center;
    padding: 3rem 1.5rem;
    background: linear-gradient(145deg, var(--aged-paper) 0%, var(--warm-paper) 100%);
    border: 1px solid var(--border-tan);
    border-radius: 16px;
    margin-top: 3rem;
  }

  .closing h2 {
    color: var(--text-brown);
    font-size: 1.5rem;
    margin-bottom: 0.75rem;
    font-weight: 600;
  }

  .closing p {
    color: var(--text-brown-light);
    max-width: 480px;
    margin: 0 auto 1.5rem;
    line-height: 1.65;
  }

  /* Responsive Adjustments */
  @media (max-width: 768px) {
    .hero {
      padding: 3rem 1.25rem;
    }

    .hero h1 {
      font-size: 2rem;
    }

    .hero .tagline {
      font-size: 1.15rem;
    }

    .hero .subtitle {
      font-size: 1rem;
    }

    .vlrb-logo {
      width: 100px;
      height: 100px;
    }

    .features {
      grid-template-columns: 1fr;
    }

    .pricing-tiers {
      grid-template-columns: 1fr;
    }

    .tier.featured {
      order: -1;
    }

    .section-title {
      font-size: 1.5rem;
    }
  }

  /* Reduced motion for accessibility */
  @media (prefers-reduced-motion: reduce) {
    .feature,
    .tier,
    .faq-item,
    .cta-button {
      transition: none;
    }

    .feature:hover,
    .cta-button:hover {
      transform: none;
    }
  }
</style>

<div class="hero">
  <div class="logo-container">
    <img src="/assets/images/vlrb-logo-dark.svg" alt="vlrb logo" class="vlrb-logo">
  </div>
  <h1>vlrb</h1>
  <p class="tagline">Stories beyond words</p>
  <p class="subtitle">Share the moments that text can't capture. Send video letters to the people who matter most, like passing a note to a dear friend.</p>
  <a href="{{ site.app_store_url }}" class="cta-button">Download on App Store</a>
</div>

<div class="section-divider">
  <span class="icon">~</span>
</div>

<section class="features-section">
  <h2 class="section-title">Made for meaningful moments</h2>
  <p class="section-subtitle">Not another social feed. Just you and the people you care about.</p>

  <div class="features">
    <article class="feature">
      <div class="feature-icon">~</div>
      <h3>Light as a letter</h3>
      <p>Videos live in the cloud, not on your phone. Share as many moments as you want without worrying about storage.</p>
    </article>

    <article class="feature">
      <div class="feature-icon">~</div>
      <h3>Take your time</h3>
      <p>Say everything you need to say. Share videos up to 10 minutes long, because some stories need room to breathe.</p>
    </article>

    <article class="feature">
      <div class="feature-icon">~</div>
      <h3>Real connection</h3>
      <p>See their smile. Hear their laugh. Share the warmth that only face-to-face can bring, even from far away.</p>
    </article>

    <article class="feature">
      <div class="feature-icon">~</div>
      <h3>Just between us</h3>
      <p>Your moments stay private. No public feeds, no algorithms, no ads. Just the people you choose to share with.</p>
    </article>
  </div>
</section>

<div class="section-divider">
  <span class="icon">~</span>
</div>

<section class="pricing">
  <h2 class="section-title">Choose your pace</h2>
  <p class="pricing-intro">Whether you send a quick hello or a heartfelt story, there's a way to connect that fits you.</p>

  <div class="pricing-tiers">
    <article class="tier">
      <div class="tier-icon">~</div>
      <h3>Free</h3>
      <div class="price">$0<span class="period"> forever</span></div>
      <p class="price-note">Start connecting today</p>
      <ul>
        <li>Videos up to 5 minutes</li>
        <li>Cloud storage for your vlrbs</li>
        <li>Clean, ad-free experience</li>
        <li>Share with anyone</li>
      </ul>
    </article>

    <article class="tier featured">
      <div class="tier-icon">~</div>
      <h3>Social</h3>
      <div class="price">{{ site.social_price_monthly }}<span class="period">/month</span></div>
      <p class="price-note">Or {{ site.social_price_yearly }}/year</p>
      <ul>
        <li>Everything in Free</li>
        <li>Videos up to 10 minutes</li>
        <li>"Live Now" so friends can watch along</li>
        <li>3 extra minutes per week when you need them</li>
      </ul>
    </article>

    <article class="tier">
      <div class="tier-icon">~</div>
      <h3>Creator</h3>
      <div class="price">{{ site.creator_price_monthly }}<span class="period">/month</span></div>
      <p class="price-note">Or {{ site.creator_price_yearly }}/year</p>
      <ul>
        <li>Everything in Social</li>
        <li>Unlimited extra time</li>
        <li>Custom expiration settings</li>
        <li>Picture-in-Picture viewing</li>
      </ul>
    </article>
  </div>
</section>

<div class="section-divider">
  <span class="icon">~</span>
</div>

<section class="faq">
  <h2 class="section-title">Questions & Answers</h2>
  <p class="section-subtitle">Everything you might want to know</p>

  <article class="faq-item">
    <h4>How is vlrb different from other video apps?</h4>
    <p>We're not trying to be a social network. vlrb is for the conversations that matter most, the ones you'd have over a cup of tea or a long phone call. No followers, no feeds, just genuine connection with the people you choose.</p>
  </article>

  <article class="faq-item">
    <h4>Will videos fill up my phone?</h4>
    <p>Not at all. Your vlrbs live in the cloud by default. You can watch them anytime, and only download the ones you want to keep forever. It's like having a shoebox of treasured letters, but the shoebox takes up no space.</p>
  </article>

  <article class="faq-item">
    <h4>What happens when videos expire?</h4>
    <p>Like letters that find their time, expired vlrbs are gently removed from our servers. With our Creator tier, you can choose when that happens. We recommend saving anything truly precious to your camera roll.</p>
  </article>

  <article class="faq-item">
    <h4>Is my content private?</h4>
    <p>Completely. Your vlrbs travel safely between you and your recipients, like sealed letters. We don't peek, we don't analyze, and we certainly don't share. Your moments are yours alone.</p>
  </article>
</section>

<div class="closing">
  <h2>Ready to share something real?</h2>
  <p>Download vlrb and send your first video letter today. No account needed to start, just open and record.</p>
  <a href="{{ site.app_store_url }}" class="cta-button">Get Started</a>
</div>
