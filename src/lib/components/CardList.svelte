<main class="card-list">
	<section class="card">
		<div class="card-wrapper">
			<h2 class="plan">Basic</h2>
			<div class="pricing">
				<small>&#36;</small>
				<h3>199.99</h3>
			</div>
			<div class="detail">
				<hr />
				<p class="detail-text">500 GB Storage</p>
				<hr />
				<p class="detail-text">2 Users Allowed</p>
				<hr />
				<p class="detail-text">Send up to 3 GB</p>
				<hr />
			</div>
			<a href="https://frontendmentor.io/" target="_blank" class="detail-button">LEARN MORE</a>
		</div>
	</section>

	<section class="card recommended">
		<div class="card-wrapper">
			<h2 class="plan">Professional</h2>
			<div class="pricing">
				<small>&#36;</small>
				<h3>249.99</h3>
			</div>
			<div class="detail">
				<hr />
				<p class="detail-text">1 TB Storage</p>
				<hr />
				<p class="detail-text">5 Users Allowed</p>
				<hr />
				<p class="detail-text">Send up to 10 GB</p>
				<hr />
			</div>
			<a href="https://frontendmentor.io/" target="_blank" class="detail-button">LEARN MORE</a>
		</div>
	</section>

	<section class="card">
		<div class="card-wrapper">
			<h2 class="plan">Master</h2>
			<div class="pricing">
				<small>&#36;</small>
				<h3>399.99</h3>
			</div>
			<div class="detail">
				<hr />
				<p class="detail-text">2 TB Storage</p>
				<hr />
				<p class="detail-text">10 Users Allowed</p>
				<hr />
				<p class="detail-text">Send up to 20 GB</p>
				<hr />
			</div>
			<a href="https://frontendmentor.io/" target="_blank" class="detail-button">LEARN MORE</a>
		</div>
	</section>
</main>

<style>
	.card-list {
		display: flex;
		flex-direction: column;
		gap: 2.03125rem;
		margin-right: 1.5rem;
		margin-left: 1.5rem;
		margin-top: 5rem;
		margin-bottom: 4.5rem;
	}

	.card {
		border-radius: 10px;
		background: #fff;
		box-shadow: 0px 20px 40px 0px rgba(212, 210, 244, 0.5);
		padding-top: 1.9375rem;
		padding-right: 1.8125rem;
		padding-bottom: 1.9375rem;
		padding-left: 1.8125rem;
	}

	.plan {
		color: var(--grayish-blue);
		text-align: center;
		font-size: 1.125rem;
		font-weight: 700;
		line-height: 1.55;
	}

	.pricing {
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 7.4px;
		margin-top: 1.5rem;
		color: var(--dark-grayish-blue);
	}

	.pricing small {
		font-size: 2.5rem;
		font-weight: 700;
	}

	.pricing h3 {
		font-size: 4.5rem;
		font-weight: 700;
		line-height: 0.986;
		letter-spacing: -2.16px;
	}

	.detail {
		margin-top: 2rem;
	}

	hr {
		opacity: 0.25;
		background: #6e728e;
	}

	.detail-text {
		color: var(--grayish-blue);
		margin-top: 0.75rem;
		margin-bottom: 0.75rem;
		text-align: center;
		font-size: 0.9375rem;
		font-weight: 700;
		line-height: 1.86;
	}
	.detail-button {
		margin-top: 2rem;
		display: block;
		font-size: 0.8125rem;
		text-align: center;
		font-weight: 700;
		letter-spacing: 1.393px;
		text-decoration: none;
		border-radius: 6px;
		background: linear-gradient(135deg, #a2a7f0 0%, #696edd 100%);
		color: #fff;
		padding-top: 0.875rem;
		padding-bottom: 0.875rem;
	}

	.recommended {
		background: linear-gradient(135deg, #a2a7f0 0%, #696edd 100%);
	}
	.recommended .plan {
		color: #fff;
	}
	.recommended .pricing {
		color: #fff;
	}
	.recommended hr {
		color: #fff;
		opacity: 0.25;
	}
	.recommended .detail-text {
		color: #fff;
	}
	.recommended .detail-button {
		background: #fff;
		color: var(--end-color);
	}
</style>
