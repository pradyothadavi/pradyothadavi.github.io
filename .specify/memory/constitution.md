<!--
Sync Impact Report:
Version change: 1.0.0 → 1.1.0 (minor version bump)
Modified principles: none
Added sections: Template Maintenance (new principle VI)
Removed sections: none
Templates requiring updates:
  ✅ Updated plan-template.md constitution check section (template maintenance checks)
  ✅ Updated spec-template.md to align with al-folio requirements
  ✅ Updated tasks-template.md for al-folio upgrade task categorization
Follow-up TODOs: none
-->

# Pradyot H Adavi Personal Website Constitution

## Core Principles

### I. Performance-First (NON-NEGOTIABLE)

All features and content MUST maintain optimal performance metrics. Website MUST load in under 3 seconds on 3G connections. Images MUST be optimized and served in modern formats (WebP/AVIF with fallbacks). CSS/JS MUST be minified and critical resources inlined. Lighthouse performance score MUST remain above 90.

_Rationale: Personal websites represent professional capabilities; slow sites reflect poorly on technical competence and user experience._

### II. Design Excellence

Visual design MUST prioritize clean, minimal aesthetics with excellent typography and whitespace usage. Interactive elements MUST provide immediate feedback. Color schemes MUST maintain WCAG AA contrast standards. Layout MUST be responsive across all device sizes with mobile-first approach.

_Rationale: A sleek design creates strong first impressions and demonstrates attention to detail valued in professional contexts._

### III. Content Quality

All content MUST be professionally written, well-structured, and regularly updated. Code examples MUST be tested and functional. Publications and project descriptions MUST be accurate and current. Grammar and spelling MUST be error-free.

_Rationale: Content quality directly reflects professional competence and attention to detail._

### IV. Build Optimization

Jekyll build process MUST be optimized for speed and efficiency. Unused CSS MUST be purged automatically. Assets MUST be compressed and cached effectively. Build pipeline MUST include automated optimization steps.

_Rationale: Efficient build processes enable rapid iteration and ensure consistent optimization across deployments._

### V. Accessibility & Standards

Website MUST comply with WCAG 2.1 AA accessibility standards. Semantic HTML MUST be used throughout. SEO optimization MUST be implemented with proper meta tags, structured data, and sitemap generation.

_Rationale: Accessibility demonstrates inclusive design principles while SEO ensures professional discoverability._

### VI. Template Maintenance (NON-NEGOTIABLE)

Website MUST stay current with [al-folio template](https://github.com/alshedivat/al-folio) updates. New features and improvements MUST be evaluated and incorporated within 30 days of template release. Security updates MUST be applied within 7 days. Template customizations MUST be documented and preserved during upgrades.

_Rationale: Staying current with template updates ensures access to latest performance improvements, security patches, and feature enhancements while maintaining professional website standards._

## Performance Standards

**Load Time Requirements**:

- First Contentful Paint: <1.5s
- Largest Contentful Paint: <2.5s
- Cumulative Layout Shift: <0.1
- Time to Interactive: <3.0s

**Asset Optimization**:

- Images: WebP/AVIF with quality <85%, lazy loading enabled
- CSS: Critical path inlined, non-critical deferred
- JavaScript: Minified, tree-shaken, code-split where beneficial
- Fonts: Preloaded, font-display: swap

**Build Performance**:

- Local development build: <10s
- Production build: <30s
- Asset processing: Automated via GitHub Actions

## Development Workflow

**Content Updates**:

- All content changes MUST be previewed locally before deployment
- Images MUST be processed through optimization pipeline
- New posts MUST include proper metadata and structured data

**Feature Development**:

- Performance impact MUST be measured before and after changes
- Design changes MUST be tested across device breakpoints
- Lighthouse audits MUST pass before deployment

**Quality Gates**:

- Automated testing via GitHub Actions for build success
- Performance regression testing for significant changes
- Accessibility validation for UI modifications

**Template Maintenance**:

- Monthly monitoring of al-folio template releases and updates
- Template upgrade evaluation MUST assess impact on customizations
- Security patches MUST be prioritized and applied immediately
- Feature additions MUST be tested for performance and accessibility compliance

## Governance

This constitution supersedes all other development practices. All website modifications MUST comply with these principles. Performance regressions are considered breaking changes requiring immediate remediation.

**Amendment Process**: Constitution changes require rationale documentation, impact assessment, and template updates. Version increments follow semantic versioning: MAJOR for principle removals/redefinitions, MINOR for new principles, PATCH for clarifications.

**Compliance Review**: Monthly Lighthouse audits required, quarterly content freshness review, annual accessibility audit.

**Version**: 1.1.0 | **Ratified**: 2025-10-29 | **Last Amended**: 2025-10-29
