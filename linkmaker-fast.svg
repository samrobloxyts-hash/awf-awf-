<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" width="1" height="1" viewBox="0 0 1 1">
  <metadata><![CDATA[
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>SVG Batch Publisher</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      background: #080808;
      color: #f3f3f3;
      line-height: 1.6;
    }

    main {
      min-height: 100vh;
      padding: 3rem 1rem;
    }

    .container {
      max-width: 48rem;
      margin: 0 auto;
    }

    header {
      display: flex;
      align-items: center;
      gap: 1rem;
      margin-bottom: 2.5rem;
    }

    .icon {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 2.75rem;
      height: 2.75rem;
      border-radius: 0.5rem;
      background: #f97316;
      color: white;
    }

    h1 {
      font-size: 1.5rem;
      font-weight: 600;
      letter-spacing: -0.025em;
    }

    .subtitle {
      font-size: 0.875rem;
      color: #a3a3a3;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
      border: 1px solid #2a2a2a;
      border-radius: 0.75rem;
      background: #151515;
      padding: 1.5rem;
      box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3);
    }

    .form-group {
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
    }

    label {
      font-size: 0.875rem;
      font-weight: 500;
    }

    input[type="text"],
    input[type="password"],
    input[type="number"],
    textarea {
      background: #080808;
      border: 1px solid #2a2a2a;
      border-radius: 0.375rem;
      color: #f3f3f3;
      padding: 0.5rem 0.75rem;
      font-family: inherit;
      font-size: 0.875rem;
    }

    input[type="text"]:focus,
    input[type="password"]:focus,
    input[type="number"]:focus,
    textarea:focus {
      outline: none;
      border-color: #f97316;
      box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.15);
    }

    textarea {
      resize: vertical;
      min-height: 60px;
    }

    .help-text {
      font-size: 0.75rem;
      color: #888888;
    }

    .mode-buttons {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 0.5rem;
    }

    button {
      padding: 0.5rem 1rem;
      border: 1px solid #2a2a2a;
      border-radius: 0.375rem;
      background: #2a2a2a;
      color: #f3f3f3;
      font-size: 0.875rem;
      font-weight: 500;
      cursor: pointer;
      transition: all 0.2s;
    }

    button:hover:not(:disabled) {
      background: #3a3a3a;
      border-color: #3a3a3a;
    }

    button.active {
      background: #f97316;
      border-color: #f97316;
    }

    button:disabled {
      opacity: 0.5;
      cursor: not-allowed;
    }

    .file-input-wrapper {
      display: flex;
      align-items: center;
      gap: 0.75rem;
    }

    .file-input-wrapper button {
      flex-shrink: 0;
      padding: 0.5rem 1rem;
    }

    .file-name {
      flex: 1;
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
      font-size: 0.875rem;
      color: #a3a3a3;
    }

    input[type="file"] {
      display: none;
    }

    .submit-btn {
      background: #f97316;
      border-color: #f97316;
      padding: 0.75rem 1rem;
      font-weight: 600;
      width: 100%;
    }

    .submit-btn:hover:not(:disabled) {
      background: #ea580c;
      border-color: #ea580c;
    }

    .warning {
      font-size: 0.75rem;
      color: #f59e0b;
      margin-top: 0.25rem;
    }

    .error {
      font-size: 0.875rem;
      color: #ef4444;
      padding: 0.75rem;
      background: rgba(239, 68, 68, 0.1);
      border-radius: 0.375rem;
      border: 1px solid rgba(239, 68, 68, 0.3);
      margin-top: 0.5rem;
    }

    .success {
      font-size: 0.875rem;
      color: #10b981;
      padding: 0.75rem;
      background: rgba(16, 185, 129, 0.1);
      border-radius: 0.375rem;
      border: 1px solid rgba(16, 185, 129, 0.3);
      margin-top: 0.5rem;
    }

    .results {
      margin-top: 2rem;
      border: 1px solid #2a2a2a;
      border-radius: 0.75rem;
      background: #151515;
      padding: 1.5rem;
    }

    .results-header {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      margin-bottom: 1.5rem;
    }

    .results-title {
      font-size: 1.125rem;
      font-weight: 600;
    }

    .results-controls {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .provider-buttons {
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
    }

    .provider-buttons button {
      padding: 0.5rem 1rem;
      font-size: 0.875rem;
    }

    .copy-btn {
      padding: 0.5rem 1rem;
      background: #2a2a2a;
      border-color: #2a2a2a;
    }

    .copy-btn:hover {
      background: #3a3a3a;
    }

    .action-buttons {
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
    }

    .action-buttons button {
      flex: 1 1 10rem;
    }

    .repo-section {
      margin-bottom: 1.5rem;
    }

    .repo-header {
      font-size: 0.875rem;
      font-weight: 600;
      margin-bottom: 0.5rem;
    }

    .repo-branch {
      color: #a3a3a3;
    }

    .url-list {
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
      font-family: "Monaco", "Menlo", monospace;
      font-size: 0.75rem;
    }

    .url-item {
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
    }

    .url-item a {
      color: #f97316;
      text-decoration: none;
    }

    .url-item a:hover {
      text-decoration: underline;
    }

    .failed-section {
      margin-top: 1.5rem;
      padding: 0.75rem;
      border: 1px solid rgba(239, 68, 68, 0.3);
      border-radius: 0.375rem;
      background: rgba(239, 68, 68, 0.05);
    }

    .failed-header {
      font-weight: 600;
      color: #ef4444;
      margin-bottom: 0.5rem;
      font-size: 0.875rem;
    }

    .failed-list {
      display: flex;
      flex-direction: column;
      gap: 0.25rem;
    }

    .failed-item {
      font-size: 0.75rem;
      color: #888888;
    }

    .shortfall {
      font-size: 0.75rem;
      color: #f59e0b;
      margin-bottom: 1rem;
    }

    code {
      background: #080808;
      padding: 0.125rem 0.375rem;
      border-radius: 0.25rem;
      font-family: "Monaco", "Menlo", monospace;
      font-size: 0.85em;
    }

    .toast {
      position: fixed;
      bottom: 1rem;
      right: 1rem;
      padding: 1rem;
      border-radius: 0.5rem;
      font-size: 0.875rem;
      max-width: 20rem;
      animation: slideIn 0.3s ease-out;
      z-index: 1000;
    }

    .toast.error {
      background: #7f1d1d;
      border: 1px solid #dc2626;
      color: #fecaca;
    }

    .toast.success {
      background: #064e3b;
      border: 1px solid #059669;
      color: #a7f3d0;
    }

    .toast.info {
      background: #2a1608;
      border: 1px solid #f97316;
      color: #fed7aa;
    }

    @keyframes slideIn {
      from {
        transform: translateX(400px);
        opacity: 0;
      }
      to {
        transform: translateX(0);
        opacity: 1;
      }
    }

    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <main>
    <div class="container">
      <header>
        <div class="icon">
      <img 
  src="https://codeberg.org/HtmlLol/P2P-EMIS/raw/branch/main/download%20%281%29.png"
  width="45"
  height="40"
  alt=""
>
        </div>
        <div>
          <h1>JSdelivr bulk  Publisher</h1>
          <p class="subtitle">Top 1 ai slop websites? Also p2p owns this join the discord the code u can get but u need to make a link first </p>
        </div>
      </header>

      <form id="form">
        <div class="form-group">
          <label for="token">GitHub token</label>
          <input type="password" id="token" placeholder="ghp_..." autocomplete="off">
          <p class="help-text">Needs <code>repo</code> or <code>public_repo</code> content write access you can read the code i dont save theese also you need to go to  https://github.com/settings/tokens/new and make a classic token i like giving it full power but ig u can do what u want.
        </div>

        <div class="form-group">
          <label>Repository mode</label>
          <div class="mode-buttons">
            <button type="button" class="mode-btn active" data-mode="explicit">Pick a repo</button>
            <button type="button" class="mode-btn" data-mode="auto">AUTO repos</button>
          </div>
          <div id="mode-explicit-info">
            <input type="text" id="repo" placeholder="owner/repo" style="margin-top: 0.5rem;">
            <p class="help-text" style="margin-top: 0.5rem;">If repo hits 1,000 SVGs, rest overflow into auto-created repos.</p>
          </div>
          <div id="mode-auto-info" class="hidden">
            <p class="help-text" style="margin-top: 0.5rem;"><code>&lt;mainword&gt;-auto-1</code>, <code>-auto-2</code>, … under your account.</p>
          </div>
        </div>

        <div class="form-group">
          <label>SVG file</label>
          <div class="file-input-wrapper">
            <button type="button" id="file-btn">Choose SVG</button>
            <span class="file-name" id="file-name">No file selected</span>
          </div>
          <input type="file" id="file-input" accept=".svg,image/svg+xml">
        </div>

        <div class="form-group">
          <label for="main-words">Main words</label>
          <textarea id="main-words"></textarea>
          <p class="help-text">make this a small list of keywords for your website to show people what it is  example my site has websight, web, sight
as the main words </p>
        </div>

        <div class="form-group">
          <label for="side-words">Side words</label>
          <textarea id="side-words"></textarea>
          <p class="help-text">Comma separated. Provide most of the randomness. if u cant think of them use theese!
game, play, load, fetch, pixel, cloud, run, view, code, hub</p>
        </div>

        <div class="form-group">
          <label for="count">How many files?</label>
          <input type="number" id="count" min="1" value="10">
          <p class="help-text">Any number from 1 up. Large batches are handled efficiently; GitHub API limits and repository size still apply. </p>
          <p class="warning" id="count-warning"></p>
        </div>

        <button type="submit" class="submit-btn" id="submit-btn">Publish to GitHub</button>
      </form>

      <div id="results" class="results hidden">
        <div class="results-header">
          <div class="results-title" id="results-title"></div>
          <div class="results-controls">
            <div class="provider-buttons" id="provider-buttons"></div>
            <div class="action-buttons">
              <button type="button" class="copy-btn" id="copy-all-btn">Copy all links</button>
              <button type="button" class="copy-btn" id="download-links-btn">Download links</button>
              <button type="button" class="copy-btn" id="random-link-btn">Open random link</button>
              <button type="button" class="copy-btn" id="download-page-btn">Download webpage</button>
            </div>
          </div>
        </div>

        <p class="shortfall hidden" id="shortfall"></p>
        <div id="repos-container"></div>
        <div id="failed-container"></div>
      </div>
    </div>
  </main>

  <script>
    const CDN_PROVIDERS = {
      jsdelivr: (repo, branch, file) => `https://cdn.jsdelivr.net/gh/${repo}@${branch}/${file}`,
      gcore: (repo, branch, file) => `https://gcore.jsdelivr.net/gh/${repo}@${branch}/${file}`,
      fastly: (repo, branch, file) => `https://fastly.jsdelivr.net/gh/${repo}@${branch}/${file}`,
    };

    const API = "https://api.github.com";
    const API_VERSION = "2026-03-10";
    // GitHub's Git Trees API supports large trees. Keep batches comfortably
    // below request/object limits while avoiding thousands of API calls.
    const MAX_SVGS_PER_REPO = 100000;
    const MAX_TREE_ENTRIES = 50000;
    const MAX_TREE_PAYLOAD_BYTES = 5_500_000;
    const RETRIES = 4;

    let state = {
      mode: "explicit",
      provider: "jsdelivr",
      result: null,
    };

    const $form = document.getElementById("form");
    const $token = document.getElementById("token");
    const $repo = document.getElementById("repo");
    const $fileBtn = document.getElementById("file-btn");
    const $fileInput = document.getElementById("file-input");
    const $fileName = document.getElementById("file-name");
    const $mainWords = document.getElementById("main-words");
    const $sideWords = document.getElementById("side-words");
    const $count = document.getElementById("count");
    const $countWarning = document.getElementById("count-warning");
    const $submitBtn = document.getElementById("submit-btn");
    const $results = document.getElementById("results");
    const $resultsTitle = document.getElementById("results-title");
    const $providerButtons = document.getElementById("provider-buttons");
    const $copyAllBtn = document.getElementById("copy-all-btn");
    const $downloadLinksBtn = document.getElementById("download-links-btn");
    const $randomLinkBtn = document.getElementById("random-link-btn");
    const $downloadPageBtn = document.getElementById("download-page-btn");
    const $reposContainer = document.getElementById("repos-container");
    const $failedContainer = document.getElementById("failed-container");
    const $shortfall = document.getElementById("shortfall");

    $mainWords.value = "web, sight";
    $sideWords.value = "game, play, load, fetch, pixel, cloud, run, view, code, hub";

    document.querySelectorAll(".mode-btn").forEach(btn => {
      btn.addEventListener("click", (e) => {
        e.preventDefault();
        state.mode = btn.dataset.mode;
        document.querySelectorAll(".mode-btn").forEach(b => b.classList.remove("active"));
        btn.classList.add("active");
        document.getElementById("mode-explicit-info").classList.toggle("hidden", state.mode !== "explicit");
        document.getElementById("mode-auto-info").classList.toggle("hidden", state.mode !== "auto");
      });
    });

    $fileBtn.addEventListener("click", (e) => {
      e.preventDefault();
      $fileInput.click();
    });

    $fileInput.addEventListener("change", () => {
      const file = $fileInput.files?.[0];
      if (!file) return;
      if (!file.name.toLowerCase().endsWith(".svg")) {
        showToast("Only SVG files accepted", "error");
        $fileInput.value = "";
        return;
      }
      $fileName.textContent = file.name;
    });

    $count.addEventListener("input", () => {
      const n = Number.parseInt($count.value, 10);
      if (Number.isFinite(n) && n > 100000) {
        $countWarning.textContent = `${n.toLocaleString()} files. This can use significant browser memory and GitHub API quota.`;
        $countWarning.style.display = "block";
      } else {
        $countWarning.style.display = "none";
      }
    });

    $form.addEventListener("submit", async (e) => {
      e.preventDefault();

      const token = $token.value.trim();
      const repo = $repo.value.trim();
      const svg = $fileInput.files?.[0];
      const mainWords = splitWords($mainWords.value);
      const sideWords = splitWords($sideWords.value);
      const count = Number.parseInt($count.value, 10);

      if (!token) return showToast("Enter a GitHub token", "error");
      if (state.mode === "explicit" && !/^[^/\s]+\/[^/\s]+$/.test(repo)) {
        return showToast("Repository must look like owner/repo", "error");
      }
      if (!svg) return showToast("Upload an SVG file", "error");
      if (mainWords.length === 0) return showToast("Add at least one main word", "error");
      if (sideWords.length === 0) return showToast("Add at least one side word", "error");
      if (!Number.isSafeInteger(count) || count < 1) return showToast("Must be a whole number of 1 or higher", "error");

      $submitBtn.disabled = true;
      $submitBtn.textContent = "Reading SVG...";

      try {
        const svgContent = await svg.text();
        const result = await publishSvgs({
          token,
          mode: state.mode,
          repo,
          svg: svgContent,
          mainWords,
          sideWords,
          count,
          onProgress: (done, total, message) => {
            $submitBtn.textContent = message || `Publishing ${done.toLocaleString()} / ${total.toLocaleString()}...`;
          },
        });

        state.result = result;
        showResults(result);
        showToast(`Published ${result.publishedCount.toLocaleString()} files`, "success");
      } catch (err) {
        console.error(err);
        showToast(err instanceof Error ? err.message : "Publishing failed", "error");
      } finally {
        $submitBtn.disabled = false;
        $submitBtn.textContent = "Publish to GitHub";
      }
    });

    function splitWords(s) {
      return [...new Set(String(s).split(",").map(w => w.trim()).filter(Boolean))];
    }

    function sleep(ms) {
      return new Promise(resolve => setTimeout(resolve, ms));
    }

    function authHeaders(token) {
      return {
        "Authorization": `Bearer ${token}`,
        "Accept": "application/vnd.github+json",
        "X-GitHub-Api-Version": API_VERSION,
      };
    }

    async function readError(response) {
      const text = await response.text().catch(() => "");
      if (!text) return `${response.status} ${response.statusText || "GitHub API error"}`;
      try {
        const json = JSON.parse(text);
        if (json?.message) return `${json.message}${json.documentation_url ? ` (${json.documentation_url})` : ""}`;
      } catch (_) {}
      return text.slice(0, 1000);
    }

    function retryDelay(response, attempt) {
      const retryAfter = Number.parseInt(response.headers.get("retry-after"), 10);
      if (Number.isFinite(retryAfter)) return Math.min(30_000, retryAfter * 1000);
      return Math.min(8_000, 500 * (2 ** attempt) + Math.floor(Math.random() * 250));
    }

    async function githubFetch(url, token, options = {}) {
      let lastError = null;
      for (let attempt = 0; attempt <= RETRIES; attempt++) {
        try {
          const response = await fetch(url, {
            ...options,
            headers: {
              ...authHeaders(token),
              ...(options.headers || {}),
            },
          });

          const retryable = response.status === 429 || response.status === 502 || response.status === 503 || response.status === 504 ||
            (response.status === 403 && response.headers.get("x-ratelimit-remaining") === "0");

          if (retryable && attempt < RETRIES) {
            await sleep(retryDelay(response, attempt));
            continue;
          }

          if (!response.ok) {
            const detail = await readError(response);
            throw new Error(`GitHub API ${response.status}: ${detail}`);
          }
          return response;
        } catch (err) {
          lastError = err;
          const isNetworkError = err instanceof TypeError || /network|fetch/i.test(String(err?.message || ""));
          if (!isNetworkError || attempt >= RETRIES) throw err;
          await sleep(Math.min(8_000, 500 * (2 ** attempt) + Math.floor(Math.random() * 250)));
        }
      }
      throw lastError || new Error("GitHub request failed");
    }

    async function githubJson(url, token, options = {}) {
      const response = await githubFetch(url, token, options);
      return response.json();
    }

    async function publishSvgs(data) {
      let response;
      try {
        response = await githubFetch(`${API}/user`, data.token);
      } catch (e) {
        throw new Error(`Could not reach GitHub: ${e instanceof Error ? e.message : String(e)}`);
      }

      const user = await response.json();
      const owner = user.login;
      const baseName = toSlug(data.mainWords[0]);
      const contentBase64 = bytesToBase64(new TextEncoder().encode(data.svg));

      const repos = [];
      const repoResults = [];
      const links = [];
      const failed = [];
      let remaining = data.count;
      let nextAutoRepo = 1;
      let globalCounter = 1;

      // Explicit mode uses the chosen repository first, then spills only the overflow
      // into <main>-auto-N repositories. AUTO mode starts there immediately.
      if (data.mode === "explicit") {
        const explicit = await loadRepo(data.repo, data.token);
        if (!explicit) throw new Error(`Repository not found: ${data.repo}`);
        repos.push(explicit);
        globalCounter = Math.max(globalCounter, explicit.maxNumber + 1);
      }

      while (remaining > 0) {
        let repoState = repos[repos.length - 1];

        if (!repoState || repoState.free <= 0 || repoState === repos[0] && data.mode === "explicit" && repos.length > 1) {
          repoState = null;
        }

        if (!repoState || (data.mode === "explicit" && repoState === repos[0] && remaining > repoState.free)) {
          // In explicit mode, finish the selected repository before creating AUTO repos.
          if (data.mode === "explicit" && repos.length === 1 && repos[0].free > 0) {
            repoState = repos[0];
          } else {
            repoState = null;
          }
        }

        if (!repoState) {
          while (true) {
            const name = `${baseName}-auto-${nextAutoRepo}`;
            nextAutoRepo++;
            let candidate = await loadRepo(`${owner}/${name}`, data.token);
            if (!candidate) {
              await createRepo(name, data.token);
              // GitHub can take a moment to expose the newly initialized branch.
              for (let attempt = 0; attempt < 6 && !candidate; attempt++) {
                if (attempt) await sleep(250 * attempt);
                candidate = await loadRepo(`${owner}/${name}`, data.token);
              }
              if (!candidate) throw new Error(`Repository ${owner}/${name} was created but its Git branch is not ready yet.`);
            }
            if (candidate.free > 0) {
              repoState = candidate;
              break;
            }
          }
          repos.push(repoState);
        }

        const targetCount = Math.min(remaining, repoState.free, MAX_SVGS_PER_REPO);
        if (targetCount <= 0) {
          repoState = null;
          continue;
        }

        data.onProgress?.(data.count - remaining, data.count, `Preparing ${targetCount.toLocaleString()} files for ${repoState.fullName}...`);

        const generated = new Array(targetCount);
        let cursor = Math.max(1, repoState.maxNumber + 1, globalCounter);
        let generatedCount = 0;

        // Existing SVGs are tracked by maxNumber. Only fall back to the Set
        // when a collision is actually possible.
        const existing = repoState.svgs;
        while (generatedCount < targetCount) {
          const candidate = `${baseName}-${cursor}.svg`.toLowerCase();
          cursor++;

          if (existing.has(candidate)) continue;
          generated[generatedCount++] = candidate;
        }
        globalCounter = cursor;

        try {
          const committed = await publishTreeBatch({
            token: data.token,
            repo: repoState,
            fileNames: generated,
            svg: data.svg,
            onProgress: completedInRepo => {
              const done = data.count - remaining + completedInRepo;
              data.onProgress?.(done, data.count, `Publishing ${done.toLocaleString()} / ${data.count.toLocaleString()}...`);
            },
          });

          for (const name of committed.names) {
            repoState.svgs.add(name);
            links.push({ repo: repoState.fullName, branch: repoState.branch, file: name });
          }

          const published = committed.names.length;
          remaining -= published;
          repoState.free = Math.max(0, MAX_SVGS_PER_REPO - repoState.svgs.size);
          for (const n of committed.names) {
            const match = n.match(/-(\d+)\.svg$/i);
            if (match) repoState.maxNumber = Math.max(repoState.maxNumber, Number(match[1]));
          }

          if (published > 0) {
            repoResults.push({ repo: repoState.fullName, branch: repoState.branch, names: committed.names });
          }

          if (published !== generated.length) {
            for (const name of generated) {
              if (!committed.names.includes(name)) {
                failed.push({ name, repo: repoState.fullName, error: "The batch was only partially committed." });
              }
            }
          }

          if (published === 0) {
            throw new Error(`No files were published to ${repoState.fullName}.`);
          }
        } catch (e) {
          for (const name of generated) {
            failed.push({ name, repo: repoState.fullName, error: e instanceof Error ? e.message : String(e) });
          }
          // Do not loop forever after a hard failure.
          break;
        }

        // If the explicit repo is now full, next iteration automatically moves to AUTO.
        if (data.mode === "explicit" && repoState === repos[0] && remaining > 0 && repoState.free === 0) {
          continue;
        }

        if (repoState.free === 0 && remaining > 0) {
          continue;
        }
        if (remaining > 0 && data.mode === "auto") {
          repoState = null;
        }
      }

      return {
        owner,
        requested: data.count,
        publishedCount: links.length,
        repos: repoResults,
        links,
        failed,
        shortfall: Math.max(0, data.count - links.length),
      };
    }

    async function loadRepo(fullName, token) {
      let info;
      try {
        info = await githubJson(`${API}/repos/${fullName}`, token);
      } catch (e) {
        if (/GitHub API 404:/i.test(String(e?.message || ""))) return null;
        throw e;
      }

      const branch = info.default_branch || "main";
      const files = await getRepoFiles(fullName, branch, token);
      const svgs = new Set();
      let maxNumber = 0;

      for (const fileName of files) {
        if (!/\.svg$/i.test(fileName)) continue;
        const lower = fileName.toLowerCase();
        svgs.add(lower);
        const match = lower.match(/-(\d+)\.svg$/);
        if (match) maxNumber = Math.max(maxNumber, Number.parseInt(match[1], 10));
      }

      return {
        fullName,
        branch,
        svgs,
        maxNumber,
        free: Math.max(0, MAX_SVGS_PER_REPO - svgs.size),
      };
    }

    async function getRepoFiles(fullName, branch, token) {
      try {
        const ref = await githubJson(`${API}/repos/${fullName}/git/ref/heads/${encodeURIComponent(branch)}`, token);
        const commit = await githubJson(`${API}/repos/${fullName}/git/commits/${ref.object.sha}`, token);
        const tree = await githubJson(`${API}/repos/${fullName}/git/trees/${commit.tree.sha}?recursive=1`, token);
        if (!tree.truncated && Array.isArray(tree.tree)) {
          return tree.tree.filter(x => x.type === "blob").map(x => x.path);
        }
      } catch (e) {
        // Fall back to the Contents API if the repository is empty or the recursive tree is truncated.
        console.warn(`Tree scan fallback for ${fullName}:`, e);
      }
      return listFiles(`${API}/repos/${fullName}/contents`, token);
    }

    async function listFiles(url, token, acc = []) {
      const response = await githubFetch(`${url}${url.includes("?") ? "&" : "?"}per_page=100`, token);
      const items = await response.json();
      if (!Array.isArray(items)) return acc;
      acc.push(...items.filter(x => x.type === "file").map(x => x.name));
      const link = response.headers.get("link");
      const next = link?.match(/<([^>]+)>;\s*rel="next"/)?.[1];
      if (next) return listFiles(next, token, acc);
      return acc;
    }

    async function createRepo(name, token) {
      const response = await githubFetch(`${API}/user/repos`, token, {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          name,
          description: "SVG batch publisher output",
          auto_init: true,
          private: false,
        }),
      });
      return response.json();
    }

    async function getGitHead(repo, token) {
      const ref = await githubJson(`${API}/repos/${repo.fullName}/git/ref/heads/${encodeURIComponent(repo.branch)}`, token);
      const commit = await githubJson(`${API}/repos/${repo.fullName}/git/commits/${ref.object.sha}`, token);
      return { commitSha: ref.object.sha, treeSha: commit.tree.sha };
    }

    async function publishTreeBatch({ token, repo, fileNames, svg, onProgress }) {
      // Create ONE blob for the SVG, then reference that blob from every file.
      // The old implementation embedded the full SVG into every tree entry,
      // making huge batches unnecessarily large and slow.
      const svgBytes = new TextEncoder().encode(svg);
      const svgBase64 = bytesToBase64(svgBytes);

      const blob = await githubJson(`${API}/repos/${repo.fullName}/git/blobs`, token, {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          content: svgBase64,
          encoding: "base64",
        }),
      });

      const head = await getGitHead(repo, token);
      let baseTreeSha = head.treeSha;
      const batches = splitTreeEntries(fileNames, blob.sha);
      let completed = 0;

      for (const entries of batches) {
        const tree = await githubJson(`${API}/repos/${repo.fullName}/git/trees`, token, {
          method: "POST",
          headers: { "Content-Type": "application/json" },
          body: JSON.stringify({
            base_tree: baseTreeSha,
            tree: entries,
          }),
        });

        baseTreeSha = tree.sha;
        completed += entries.length;
        onProgress?.(completed);
      }

      const commit = await githubJson(`${API}/repos/${repo.fullName}/git/commits`, token, {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          message: `Add ${completed} SVG file${completed === 1 ? "" : "s"}`,
          tree: baseTreeSha,
          parents: [head.commitSha],
        }),
      });

      try {
        await githubJson(`${API}/repos/${repo.fullName}/git/refs/heads/${encodeURIComponent(repo.branch)}`, token, {
          method: "PATCH",
          headers: { "Content-Type": "application/json" },
          body: JSON.stringify({
            sha: commit.sha,
            force: false,
          }),
        });
      } catch (e) {
        throw new Error(
          `Commit ${commit.sha} was created but the ${repo.branch} branch could not be updated: ${
            e instanceof Error ? e.message : String(e)
          }`
        );
      }

      return { names: fileNames };
    }

    function splitTreeEntries(fileNames, blobSha) {
      const entries = [];
      let batch = [];
      let bytes = 0;

      for (const file of fileNames) {
        const entry = {
          path: file,
          mode: "100644",
          type: "blob",
          sha: blobSha,
        };

        // Estimate request size without repeatedly encoding the SVG itself.
        const entryBytes = JSON.stringify(entry).length + 32;

        if (
          batch.length > 0 &&
          (batch.length >= MAX_TREE_ENTRIES ||
            bytes + entryBytes > MAX_TREE_PAYLOAD_BYTES)
        ) {
          entries.push(batch);
          batch = [];
          bytes = 0;
        }

        batch.push(entry);
        bytes += entryBytes;
      }

      if (batch.length) entries.push(batch);
      return entries;
    }

    function bytesToBase64(bytes) {
      let binary = "";
      const chunkSize = 0x8000;
      for (let i = 0; i < bytes.length; i += chunkSize) {
        binary += String.fromCharCode(...bytes.subarray(i, i + chunkSize));
      }
      return btoa(binary);
    }

    function toSlug(s) {
      return String(s).toLowerCase().replace(/[^a-z0-9-]+/g, "-").replace(/^-+|-+$/g, "") || "svg";
    }

    function showResults(result) {
      $results.classList.remove("hidden");
      $resultsTitle.textContent = `Published ${result.publishedCount.toLocaleString()} of ${result.requested.toLocaleString()}`;

      $providerButtons.innerHTML = "";
      Object.keys(CDN_PROVIDERS).forEach(provider => {
        const btn = document.createElement("button");
        btn.type = "button";
        btn.textContent = provider === "gcore" ? "Gcore" : provider === "fastly" ? "Fastly" : "jsDelivr";
        btn.className = provider === state.provider ? "active" : "";
        btn.addEventListener("click", (e) => {
          e.preventDefault();
          state.provider = provider;
          document.querySelectorAll("#provider-buttons button").forEach(b => b.classList.remove("active"));
          btn.classList.add("active");
          renderRepos(result);
        });
        $providerButtons.appendChild(btn);
      });

      if (result.shortfall > 0) {
        $shortfall.classList.remove("hidden");
        $shortfall.textContent = `${result.shortfall.toLocaleString()} file${result.shortfall === 1 ? "" : "s"} could not be placed.`;
      } else {
        $shortfall.classList.add("hidden");
      }

      renderRepos(result);

      if (result.failed.length > 0) {
        $failedContainer.innerHTML = `
          <div class="failed-section">
            <div class="failed-header">${result.failed.length.toLocaleString()} failed</div>
            <div class="failed-list">
              ${result.failed.slice(0, 20).map(f => `<div class="failed-item">${escapeHtml(f.repo)}/${escapeHtml(f.name)}: ${escapeHtml(f.error)}</div>`).join("")}
            </div>
          </div>
        `;
      } else {
        $failedContainer.innerHTML = "";
      }
    }

    function renderRepos(result) {
      const providerFn = CDN_PROVIDERS[state.provider];
      const fragment = document.createDocumentFragment();
      const DISPLAY_LIMIT = 1000;

      result.repos.forEach(r => {
        const section = document.createElement("div");
        section.className = "repo-section";

        const header = document.createElement("div");
        header.className = "repo-header";
        header.textContent = `${r.repo} `;

        const branch = document.createElement("span");
        branch.className = "repo-branch";
        branch.textContent = `@${r.branch}`;

        header.appendChild(branch);
        header.appendChild(
          document.createTextNode(
            ` — ${r.names.length.toLocaleString()} file${r.names.length === 1 ? "" : "s"}`
          )
        );
        section.appendChild(header);

        const list = document.createElement("div");
        list.className = "url-list";

        const visible = r.names.length > DISPLAY_LIMIT
          ? r.names.slice(0, DISPLAY_LIMIT)
          : r.names;

        for (const n of visible) {
          const url = providerFn(r.repo, r.branch, n);
          const row = document.createElement("div");
          row.className = "url-item";

          const a = document.createElement("a");
          a.href = url;
          a.target = "_blank";
          a.rel = "noopener noreferrer";
          a.textContent = url;

          row.appendChild(a);
          list.appendChild(row);
        }

        if (r.names.length > DISPLAY_LIMIT) {
          const note = document.createElement("div");
          note.className = "help-text";
          note.textContent =
            `Showing the first ${DISPLAY_LIMIT.toLocaleString()} links. ` +
            `Use "Copy all links" or "Download links" for all ${r.names.length.toLocaleString()}.`;
          section.appendChild(list);
          section.appendChild(note);
        } else {
          section.appendChild(list);
        }

        fragment.appendChild(section);
      });

      $reposContainer.replaceChildren(fragment);
    }

    function getAllLinks() {
      if (!state.result) return [];
      const providerFn = CDN_PROVIDERS[state.provider];
      const links = new Array(state.result.links.length);
      for (let i = 0; i < state.result.links.length; i++) {
        const x = state.result.links[i];
        links[i] = providerFn(x.repo, x.branch, x.file);
      }
      return links;
    }

    function downloadText(filename, text, type = "text/plain;charset=utf-8") {
      const blob = new Blob([text], { type });
      const url = URL.createObjectURL(blob);
      const a = document.createElement("a");
      a.href = url;
      a.download = filename;
      document.body.appendChild(a);
      a.click();
      a.remove();
      setTimeout(() => URL.revokeObjectURL(url), 0);
    }

    $copyAllBtn.addEventListener("click", async (e) => {
      e.preventDefault();
      const links = getAllLinks();
      if (!links.length) return showToast("No links to copy yet", "error");
      try {
        await navigator.clipboard.writeText(links.join("\n"));
        showToast(`${links.length.toLocaleString()} links copied (${state.provider})`, "success");
      } catch {
        showToast("Clipboard access failed", "error");
      }
    });

    $downloadLinksBtn.addEventListener("click", () => {
      const links = getAllLinks();
      if (!links.length) return showToast("No links to download yet", "error");
      downloadText(`svg-links-${state.provider}.txt`, links.join("\n") + "\n");
      showToast(`Downloading ${links.length.toLocaleString()} links`, "success");
    });

    $randomLinkBtn.addEventListener("click", () => {
      const links = getAllLinks();
      if (!links.length) return showToast("No links available yet", "error");
      const url = links[Math.floor(Math.random() * links.length)];
      window.open(url, "_blank", "noopener");
    });

    $downloadPageBtn.addEventListener("click", () => {
      // Download the application itself without exporting the entered token or results.
      const clone = document.documentElement.cloneNode(true);
      const token = clone.querySelector("#token");
      if (token) token.value = "";
      const results = clone.querySelector("#results");
      if (results) {
        results.classList.add("hidden");
        results.querySelector("#repos-container")?.replaceChildren();
        results.querySelector("#failed-container")?.replaceChildren();
      }
      const warning = clone.querySelector("#count-warning");
      if (warning) warning.textContent = "";
      downloadText("svg-batch-publisher.html", "<!DOCTYPE html>\n" + clone.outerHTML, "text/html;charset=utf-8");
      showToast("Webpage downloaded", "success");
    });

    function showToast(msg, type = "info") {
      const toast = document.createElement("div");
      toast.className = `toast ${type}`;
      toast.textContent = msg;
      document.body.appendChild(toast);
      setTimeout(() => toast.remove(), 4000);
    }
</script>
</body>
</html>

  ]]></metadata>
</svg>
