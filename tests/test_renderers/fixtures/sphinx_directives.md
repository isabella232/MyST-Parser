--------------------------------
default-role (`sphinx.directives.DefaultRole`):
.
```{default-role}
```
.
<document source="notset">
.

--------------------------------
default-domain (`sphinx.directives.DefaultDomain`):
.
```{default-domain} mydomain
```
.
<document source="notset">
.

--------------------------------
SPHINX4 object (`sphinx.directives.ObjectDescription`):
.
```{object} something
```
.
<document source="notset">
    <index entries="">
    <desc classes="object" desctype="object" domain="" noindex="False" objtype="object">
        <desc_signature classes="sig sig-object">
            <desc_name classes="sig-name descname" xml:space="preserve">
                something
        <desc_content>
.

--------------------------------
highlight (`sphinx.directives.code.Highlight`):
.
```{highlight} something
```
.
<document source="notset">
    <highlightlang force="False" lang="something" linenothreshold="9223372036854775807">
.

--------------------------------
code-block (`sphinx.directives.code.CodeBlock`):
.
```{code-block}
:dedent:

    a=1
```
.
<document source="notset">
    <literal_block force="False" highlight_args="{}" language="default" xml:space="preserve">
        a=1
.

--------------------------------
sourcecode (`sphinx.directives.code.CodeBlock`):
.
```{sourcecode}
```
.
<document source="notset">
    <literal_block force="False" highlight_args="{}" language="default" xml:space="preserve">
.

--------------------------------
literalinclude (`sphinx.directives.code.LiteralInclude`):
SKIP: Tested in sphinx builds
.
```{literalinclude} /path/to/file
```
.
<document source="notset">
    <system_message level="2" line="1" source="notset" type="WARNING">
        <paragraph>
            Include file '/srcdir/path/to/file' not found or reading it failed
.

--------------------------------
toctree (`sphinx.directives.other.TocTree`):
.
```{toctree}
```
.
<document source="notset">
    <compound classes="toctree-wrapper">
        <toctree caption="True" entries="" glob="False" hidden="False" includefiles="" includehidden="False" maxdepth="-1" numbered="0" parent="mock_docname" titlesonly="False">
.

--------------------------------
sectionauthor (`sphinx.directives.other.Author`):
.
```{sectionauthor} bob geldof
```
.
<document source="notset">
.

--------------------------------
moduleauthor (`sphinx.directives.other.Author`):
.
```{moduleauthor} ringo starr
```
.
<document source="notset">
.

--------------------------------
codeauthor (`sphinx.directives.other.Author`):
.
```{codeauthor} paul mcartney
```
.
<document source="notset">
.

--------------------------------
index (`sphinx.directives.other.Index`):
.
```{index} something
```
.
<document source="notset">
    <index entries="('single',\ 'something',\ 'index-0',\ '',\ None)" inline="False">
    <target ids="index-0">
.

--------------------------------
seealso (`sphinx.directives.other.SeeAlso`):
.
```{seealso}

a
```
.
<document source="notset">
    <seealso>
        <paragraph>
            a
.

--------------------------------
tabularcolumns (`sphinx.directives.other.TabularColumns`):
.
```{tabularcolumns} spec
```
.
<document source="notset">
    <tabular_col_spec spec="spec">
.

--------------------------------
centered (`sphinx.directives.other.Centered`):
.
```{centered} text
```
.
<document source="notset">
    <centered>
        text
.

--------------------------------
acks (`sphinx.directives.other.Acks`):
.
```{acks}

- name
```
.
<document source="notset">
    <acks>
        <bullet_list bullet="-">
            <list_item>
                <paragraph>
                    name
.

--------------------------------
SPHINX4 hlist (`sphinx.directives.other.HList`):
.
```{hlist}

- item
```
.
<document source="notset">
    <hlist ncolumns="2">
        <hlistcol>
            <bullet_list>
                <list_item>
                    <paragraph>
                        item
        <hlistcol>
            <bullet_list>
.

--------------------------------
only (`sphinx.directives.other.Only`):
.
```{only} expr
```
.
<document source="notset">
    <only expr="expr">
.

--------------------------------
include (`sphinx.directives.other.Include`):
SKIP: Tested in sphinx builds
.
```{include} path/to/include
```
.
<document source="notset">
.

--------------------------------
figure (`sphinx.directives.patches.Figure`):
.
```{figure} path/to/figure

*caption*

legend
```
.
<document source="notset">
    <figure>
        <image uri="path/to/figure">
        <caption>
            <emphasis>
                caption
        <legend>
            <paragraph>
                legend
.

--------------------------------
meta (`sphinx.directives.patches.Meta`):
SKIP: MockingError: MockState has not yet implemented attribute 'nested_list_parse'
.
```{meta}
foo
```
.
<document source="notset">
.

--------------------------------
table (`sphinx.directives.patches.RSTTable`):
.
```{table} *title*
:name: name

| a | b |
|---|---|
| 1 | 2 |
```
.
<document source="notset">
    <table classes="colwidths-auto" ids="name" names="name">
        <title>
            <emphasis>
                title
        <tgroup cols="2">
            <colspec colwidth="50.0">
            <colspec colwidth="50.0">
            <thead>
                <row>
                    <entry>
                        <paragraph>
                            a
                    <entry>
                        <paragraph>
                            b
            <tbody>
                <row>
                    <entry>
                        <paragraph>
                            1
                    <entry>
                        <paragraph>
                            2
.

--------------------------------
csv-table (`sphinx.directives.patches.CSVTable`):
.
```{csv-table}

"Albatross", 2.99, "On a stick!"
```
.
<document source="notset">
    <table>
        <tgroup cols="3">
            <colspec colwidth="33">
            <colspec colwidth="33">
            <colspec colwidth="33">
            <tbody>
                <row>
                    <entry>
                        <paragraph>
                            Albatross
                    <entry>
                        <paragraph>
                            2.99
                    <entry>
                        <paragraph>
                            On a stick!
.

--------------------------------
list-table (`sphinx.directives.patches.ListTable`):
.
```{list-table}

* - item
```
.
<document source="notset">
    <table>
        <tgroup cols="1">
            <colspec colwidth="100">
            <tbody>
                <row>
                    <entry>
                        <paragraph>
                            item
.

--------------------------------
code (`sphinx.directives.patches.Code`):
.
```{code} python

a
```
.
<document source="notset">
    <literal_block force="False" highlight_args="{}" language="python" xml:space="preserve">
        a
.

--------------------------------
math (`sphinx.directives.patches.MathDirective`):
.
```{math}
```
.
<document source="notset">
    <math_block docname="mock_docname" label="True" nowrap="False" number="True" xml:space="preserve">
.

--------------------------------
deprecated (`sphinx.domains.changeset.VersionChange`):
.
```{deprecated} 0.3
```
.
<document source="notset">
    <versionmodified type="deprecated" version="0.3">
        <paragraph translatable="False">
            <inline classes="versionmodified deprecated">
                Deprecated since version 0.3.
.

--------------------------------
versionadded (`sphinx.domains.changeset.VersionChange`):
.
```{versionadded} 0.2
```
.
<document source="notset">
    <versionmodified type="versionadded" version="0.2">
        <paragraph translatable="False">
            <inline classes="versionmodified added">
                New in version 0.2.
.

--------------------------------
versionchanged (`sphinx.domains.changeset.VersionChange`):
.
```{versionchanged} 0.1
```
.
<document source="notset">
    <versionmodified type="versionchanged" version="0.1">
        <paragraph translatable="False">
            <inline classes="versionmodified changed">
                Changed in version 0.1.
.
--------------------------------
glossary (`sphinx.domains.std.Glossary`):
.
```{glossary}

term 1 : A
term 2 : B
    Definition of both terms.
```
.
<document source="notset">
    <glossary>
        <definition_list classes="glossary">
            <definition_list_item>
                <term ids="term-term-1">
                    term 1
                    <index entries="('single',\ 'term\ 1',\ 'term-term-1',\ 'main',\ 'A')">
                <term ids="term-term-2">
                    term 2
                    <index entries="('single',\ 'term\ 2',\ 'term-term-2',\ 'main',\ 'B')">
                <definition>
                    <paragraph>
                        Definition of both terms.
.

--------------------------------
SPHINX3 productionlist (`sphinx.domains.std.ProductionList`):
.
```{productionlist} try_stmt: try1_stmt | try2_stmt
```
.
<document source="notset">
    <productionlist>
        <production ids="grammar-token-try_stmt grammar-token-try-stmt" tokenname="try_stmt" xml:space="preserve">
             try1_stmt | try2_stmt
.

--------------------------------
SPHINX4 cmdoption (`sphinx.domains.std.Cmdoption`):
.
```{cmdoption} a
```
.
<document source="notset">
    <index entries="('pair',\ 'command\ line\ option;\ a',\ 'cmdoption-arg-a',\ '',\ None)">
    <desc classes="std cmdoption" desctype="cmdoption" domain="std" noindex="False" objtype="cmdoption">
        <desc_signature allnames="a" classes="sig sig-object" ids="cmdoption-arg-a">
            <desc_name classes="sig-name descname" xml:space="preserve">
                a
            <desc_addname classes="sig-prename descclassname" xml:space="preserve">
        <desc_content>
.

--------------------------------
SPHINX4 rst:directive (`sphinx.domains.rst.ReSTDirective`):
.
```{rst:directive} a
```
.
<document source="notset">
    <index entries="('single',\ 'a\ (directive)',\ 'directive-a',\ '',\ None)">
    <desc classes="rst directive" desctype="directive" domain="rst" noindex="False" objtype="directive">
        <desc_signature classes="sig sig-object" ids="directive-a">
            <desc_name classes="sig-name descname" xml:space="preserve">
                .. a::
        <desc_content>
.

--------------------------------
SPHINX4 rst:directive:option (`sphinx.domains.rst.ReSTDirectiveOption`):
.
```{rst:directive:option} a
```
.
<document source="notset">
    <index entries="('single',\ ':a:\ (directive\ option)',\ 'directive-option-a',\ '',\ 'A')">
    <desc classes="rst directive:option" desctype="directive:option" domain="rst" noindex="False" objtype="directive:option">
        <desc_signature classes="sig sig-object" ids="directive-option-a directive:option--a">
            <desc_name classes="sig-name descname" xml:space="preserve">
                :a:
        <desc_content>
.
