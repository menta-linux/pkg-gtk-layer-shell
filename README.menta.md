# pkg-gtk-layer-shell (Menta Linux)

Debian packaging of gtk-layer-shell 0.10.1, taken unchanged from the Debian
MATE team packaging on Salsa (debian/gtk-layer-shell, 0.10.1-1). 0.10.1 is the
current upstream release; stable (trixie) only ships 0.9.0, so this repo exists
to provide a newer build there for Menta's mate-panel (Wayland layer-shell support).

- Binary package names are identical to Debian's (libgtk-layer-shell0,
  libgtk-layer-shell-dev, gir1.2-gtklayershell-0.1, gtk-layer-shell-doc,
  gtk-layer-shell-examples), so `libgtk-layer-shell-dev (>= 0.1.0-3~)` is satisfied.
- Versioning: `<upstream>-<rev>mentaN` (0.10.1-1menta1); CI appends `~deb13` for trixie.
- Upstream tarball is fetched from the GitHub tag in CI; no Menta patches beyond
  Debian's `2001_disable-license-check-unit-test.patch`.
- CI builds on push to `master` (rolling `latest` / `latest-trixie` releases);
  tag `menta/<version>` publishes a GitHub release.
